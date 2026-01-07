---
related:
  - "[[Finance]]"
type: "[[Notes]]"
---

> [!source] ChatGPT


> [!summary] Summary
> - Unlookthrough → Collapse (e.g. Aggregate to position)
> - Lookthrough → Expand (e.g. Drill-down to trade)

This sits right at the intersection of **treasury**, **risk**, and **data lineage / consolidation** concepts.  
The term **“unlookthrough”** (sometimes “un-look-through”) appears in contexts like **fund-of-funds**, **balance sheet aggregation**, **regulatory reporting**, and **Fintigrate / ALM data ingestion** pipelines.

Let’s break it down properly 👇

---

## 💡 **Definition**

An **“unlookthrough process”** refers to a **data or aggregation step where the system _stops looking through_ the underlying components or exposures of an instrument or entity**, and instead **treats it as a single aggregated position**.

> 🧩 In simple terms:  
> A _“lookthrough”_ process expands an instrument to reveal its underlying holdings.  
> An _“unlookthrough”_ process collapses it back to the parent level.

---

## 🧭 **Conceptual Example**

Imagine you have a **fund-of-funds** structure:

### 1) Lookthrough → Unlookthrough (conceptual flow)

```mermaid

flowchart TD
	A[Portfolio / Fund-of-Funds] --> B{Lookthrough?}
	B -- Yes --> C[Decompose to Underlyings<br/>(Securities, FX legs, Cashflows)]
	C --> D[Exposure by Asset/Issuer/Currency]
	D --> E{Unlookthrough?}
	E -- Yes --> F[Aggregate back to Parent Entity<br/>(Fund / Balance Sheet Line)]
	E -- No --> D
	B -- No --> F
	
```

```vbnet
Parent Fund (Fund A)  ├── Sub-Fund 1 → holds 50% Bonds, 50% Equities  ├── Sub-Fund 2 → holds 100% Cash
```


```mermaid
flowchart LR
  A[Fund A] --> B[Sub-Fund 1]
  A --> C[Sub-Fund 2]
  B --> B1[Bonds 50%]
  B --> B2[Equities 50%]
  C --> C1[Cash 100%]

  %% Lookthrough view
  subgraph LT[Lookthrough Exposure]
    L1[Fund A → 25% Bonds]
    L2[Fund A → 25% Equities]
    L3[Fund A → 50% Cash]
  end

  %% Unlookthrough view
  subgraph ULT[Unlookthrough (Collapsed)]
    U1[Fund A (single line)]
  end

  B1 -.roll up.-> L1
  B2 -.roll up.-> L2
  C1 -.roll up.-> L3
  L1 ==> U1
  L2 ==> U1
  L3 ==> U1

```



- **Lookthrough:**  
    You “look through” Fund A to see its ultimate exposure: 25% bonds, 25% equities, 50% cash.
    
- **Unlookthrough:**  
    You _collapse_ everything back to **Fund A as a single line item** (without tracing to sub-holdings).
    

---

## ⚙️ **In Treasury / Fintigrate / ALM Context**

In the **Fintigrate** or **Treasury data consolidation** context, the **unlookthrough process** typically refers to:

|**Process Stage**|**Description**|
|---|---|
|**Lookthrough**|The ETL expands nested fund, portfolio, or derivative positions to their **underlying securities or cashflows**, using _holding hierarchies_ or _reference mappings_.|
|**Unlookthrough**|The process where these detailed exposures are **rolled back up** to the parent fund, entity, or accounting line — often to match the **reporting entity’s balance sheet view**.|

---

### 🧩 Example in Practice (Sanlam / Fintigrate Type Setup)

|**Step**|**Process**|**Result**|
|---|---|---|
|**1. HiPort / Murex data load**|Load detailed portfolio holdings and derivatives.|Each fund or portfolio has detailed security-level exposures.|
|**2. Lookthrough process**|Decompose multi-layer funds into their underlying securities and FX exposures.|Now each asset class is fully transparent.|
|**3. Unlookthrough process**|Roll up those detailed lookthrough positions to the **ultimate holding entity** (e.g. a life fund, balance sheet, or legal entity).|Provides entity-level totals for ALM, liquidity, FTP, or IFRS reporting.|

---

## 🧮 **Why It Matters**

|**Area**|**Why You Need Unlookthrough**|
|---|---|
|**Regulatory Reporting (Solvency II, Basel III)**|Some reports require both lookthrough (to see risk exposure) _and_ unlookthrough (for balance sheet consistency).|
|**ALM & FTP**|Treasury needs entity-level totals, not exploded fund holdings.|
|**Data Lineage / VODS Layer**|Keeps two perspectives: _lookthrough data_ (risk transparency) and _unlookthrough data_ (reporting alignment).|
|**Performance & Storage**|Collapsing detailed exposures reduces data volume for downstream reporting.|

---

## 📊 **Visual Summary**

         `+----------------+          |  Lookthrough   |          |  (Expand Data) |          +----------------+                 ↓      [Each fund decomposed into securities]                 ↓          +----------------+          | Unlookthrough  |          | (Aggregate Up) |          +----------------+                 ↓    [Entity-level positions for ALM, Liquidity, Reporting]`

---

## 🧠 **Summary Table**

|**Term**|**Action**|**Purpose**|
|---|---|---|
|**Lookthrough**|Expands instruments into their underlying exposures.|Risk transparency, detailed analysis.|
|**Unlookthrough**|Collapses underlying exposures back to parent or reporting level.|Aggregation, accounting alignment, ALM/FTP inputs.|

# Diagrams

## 1 Lookthrough → Unlookthrough (Conceptual Flow)

```mermaid
%%{init: {
  "theme": "base",
  "themeVariables": {
    "primaryColor": "#b0e3e8",
    "secondaryColor": "#2fcc78",
    "tertiaryColor": "#f0f0f0",
    "lineColor": "#666",
    "fontFamily": "Segoe UI",
    "fontSize": "14px"
  }
}}%%
flowchart TD
  A["Portfolio / Fund-of-Funds"] --> B{"Lookthrough?"}
  B -- Yes --> C["Decompose to Underlyings\n(Securities, FX legs, Cashflows)"]
  C --> D["Exposure by Asset / Issuer / Currency"]
  D --> E{"Unlookthrough?"}
  E -- Yes --> F["Aggregate back to Parent Entity\n(Fund / Balance Sheet Line)"]
  E -- No --> D
  B -- No --> F

```



## 2 Funds of Funds example (Numbers)

```mermaid
%%{init: {
  "theme": "base",
  "themeVariables": {
    "primaryColor": "#b0e3e8",
    "secondaryColor": "#2fcc78",
    "tertiaryColor": "#f0f0f0",
    "lineColor": "#666",
    "fontFamily": "Segoe UI",
    "fontSize": "14px"
  }
}}%%
flowchart LR
  A["Fund A"] --> B["Sub-Fund 1"]
  A --> C["Sub-Fund 2"]
  B --> B1["Bonds 50%"]
  B --> B2["Equities 50%"]
  C --> C1["Cash 100%"]

  subgraph LT["Lookthrough Exposure"]
    L1["Fund A → 25% Bonds"]
    L2["Fund A → 25% Equities"]
    L3["Fund A → 50% Cash"]
  end

  subgraph ULT["Unlookthrough (Collapsed)"]
    U1["Fund A (single line)"]
  end

  B1 -. roll up .-> L1
  B2 -. roll up .-> L2
  C1 -. roll up .-> L3
  L1 -. aggregate .-> U1
  L2 -. aggregate .-> U1
  L3 -. aggregate .-> U1

```


## 3 Fintigrate + Murex + VODS (incl. RTBS & RTNS)

```mermaid
flowchart TD
  subgraph Sources
    HP["HiPort Holdings"]
    MX["Murex MX.3"]
    HANA["SAP HANA GL"]
    MD["Market Data: Curves / FX"]
  end

  subgraph Murex_RT["Real-Time Layer"]
    RTBS["RTBS\nReal-Time Blotter Server"]
  end

  subgraph ETL["ETL / Ingestion"]
    GLUE["AWS Glue Jobs"]
    LOAD["Load & Harmonize"]
  end

  subgraph VODS["Valuation & Operational Data Store"]
    VAL["Valuations"]
    OPS["Operational Metadata\n(repdate, version, lineage)"]
    LTBL["Lookthrough Tables"]
    ULTBL["Unlookthrough Tables"]
  end

  subgraph Downstream["Analytics / Reporting"]
    RS["Redshift Data Marts"]
    PBI["Power BI / Dashboards"]
    ALM["ALM / Liquidity / FTP"]
    RTNS["RTNS\nReal-Time Net Settlement"]
  end

  MX --> RTBS
  RTBS -->|Trade/Position Events| GLUE
  HP --> GLUE
  MX --> GLUE
  HANA --> GLUE
  MD --> GLUE

  GLUE --> LOAD --> VODS
  VODS --> RS --> PBI
  VODS --> ALM
  ALM --> RTNS

```




## 4 Lookthrough / Unlookthrough data transformation (ETL stages)


```mermaid
flowchart LR
  S1["Raw Positions & Trades"] --> S2["Normalize Entities & IDs"]
  S2 --> S3["Map Hierarchies\n(Fund ↔ Holdings)"]
  S3 --> S4["Lookthrough Expansion\n(explode to underlyings)"]
  S4 --> S5["Risk Classification\n(Asset, Sector, FX)"]
  S5 --> S6["Unlookthrough Roll-up\n(aggregate to parent/entity)"]
  S6 --> S7["Publish to VODS:\nLT tables & ULT tables"]
  S7 --> S8["Downstream:\nALM / FTP / Reporting"]


```


## 5 Sequence (booking → RTBS → VODS → report)

```mermaid
sequenceDiagram
  autonumber
  participant Trader
  participant Murex as Murex MX.3
  participant RTBS as RTBS
  participant ETL as ETL/Glue
  participant VODS
  participant BI as Reports/ALM

  Trader->>Murex: Book/Amend Trade
  Murex-->>RTBS: Emit real-time event
  RTBS-->>ETL: Publish trade/position update
  ETL->>VODS: Validate + harmonize + store
  ETL->>VODS: Update Lookthrough/Unlookthrough tables
  VODS-->>BI: Serve datasets (positions, valuations)
  BI-->>Trader: Dashboards / Risk / ALM views

```

## 6 State view: Position Representation

```mermaid
stateDiagram-v2
  [*] --> Collapsed
  Collapsed: Unlookthrough (Parent-level)
  Collapsed --> Expanded: Run Lookthrough
  Expanded: Underlying-level exposures
  Expanded --> Collapsed: Run Unlookthrough (Roll-up)

```
