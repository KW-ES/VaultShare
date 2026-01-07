---
type: "[[Notes]]"
related:
  - "[[Business Analysis]]"
---
When you’re reading _many documents_ (legacy specs, contracts, procedures, policy manuals, business rules, system outputs, etc.), it’s easy to drown in detail and miss the _true business requirements_.

Below is a structured way to **read analytically** — _extracting requirements instead of merely absorbing information._

---

## 🧭 1. The “Mental Filters” to Keep in Your Head

Think of these as lenses you continuously switch between while reading.

|Lens|Question to Keep in Mind|What You’re Looking For|
|---|---|---|
|🎯 **Purpose Lens**|“Why does this document/process exist?”|The _business objective_ behind the text|
|👥 **Actor Lens**|“Who performs this step?”|Roles, responsibilities, ownership|
|⚙️ **Process Lens**|“What are the inputs, transformations, and outputs?”|Core workflow logic|
|🧩 **Rule Lens**|“What decisions or validations happen here?”|Business rules, constraints, conditions|
|🧾 **Data Lens**|“What data is created, modified, or referenced?”|Entities, attributes, data dependencies|
|🧱 **System Lens**|“Where does technology enable or restrict this?”|Existing system functionality and gaps|
|🔄 **Change Lens**|“What could fail or need improvement?”|Gaps, pain points, inefficiencies|
|📈 **Value Lens**|“What business value is protected or created here?”|KPIs, ROI, cost/benefit reasoning|

🧠 _These lenses act like categories in your notes — every insight can be dropped into one bucket._

---

## 🧰 2. Framework for Extracting Requirements from Documents

|Step|What to Do|Example|
|---|---|---|
|**1️⃣ Skim for Structure**|Read headings, TOC, section titles first|Identify “scope,” “process,” “inputs”|
|**2️⃣ Highlight Verbs**|Circle verbs like “must,” “shall,” “will,” “may”|"System shall validate…” → functional requirement|
|**3️⃣ Identify Nouns**|Entities = Data points|“Customer,” “Loan,” “Account,” etc.|
|**4️⃣ Watch for Business Rules**|Conditional logic or thresholds|“If balance < 0, reject transaction”|
|**5️⃣ Note Stakeholders Mentioned**|Every actor or department = stakeholder to engage|“Operations team,” “Compliance officer”|
|**6️⃣ Find Metrics & Controls**|Quantitative values or tolerances|“Must complete within 2 business days”|
|**7️⃣ Map Inputs → Outputs**|For every process described|“Receive file → Validate → Store → Report”|
|**8️⃣ Look for Exceptions**|Deviations = gold for requirements|“Unless flagged by compliance…”|

---

## 🗂️ 3. How to Organize Your Findings (While Reading)

Use a **Requirements Extraction Matrix** — even a spreadsheet works.

|Doc Source|Page/Section|Entity / Process|Extracted Requirement|Type (F/NF/Rule)|Notes / Clarifications|
|---|---|---|---|---|---|
|Policy A|12|Account Opening|Customer ID must be verified via KYC|Functional / Rule|Confirm with Compliance|
|Procedure B|5|Data Upload|File accepted only if size < 10MB|Non-functional|Clarify limit justification|
|SLA C|3|Transaction Processing|95% success within 2 hours|NFR / Performance|Metric for monitoring|

This prevents duplication and supports _traceability later._

---

## 🧩 4. Distinguish Requirement Types as You Read

|Category|Description|Example|
|---|---|---|
|**Business Requirement (BR)**|The _why_ — strategic or high-level goal|“Improve client onboarding efficiency”|
|**Stakeholder Requirement (SR)**|The _who_ — what specific users need|“Ops users want auto-validation of forms”|
|**Functional Requirement (FR)**|The _what_ — system capability|“System must calculate accrued interest daily”|
|**Non-Functional (NFR)**|The _how well_ — quality attributes|“System uptime 99.5%”|
|**Transition Requirement (TR)**|Temporary or migration needs|“Migrate last 2 years of customer data”|

👉 As you read documents, tag each note with its type — this habit clarifies intent early.

---

## 🧭 5. Signs You’ve Found a True Requirement

✅ It expresses a **need or constraint**, not just a fact.  
✅ It can be **tested or verified**.  
✅ It has a **source (stakeholder, policy, system)**.  
✅ It contributes to a **business goal or KPI**.  
✅ It’s stated in a way that a designer/developer can act on.

Example:

> ❌ “Customers submit forms manually.”  
> ✅ “System must allow customers to upload forms electronically.”

---

## 🧠 6. Meta-Strategy — Reading in Layers

Think of document review like **peeling an onion**:

1. **Pass 1 — Surface Understanding**  
    → What’s the general process and scope?
2. **Pass 2 — Functional Extraction**  
    → What actions, rules, data are described?
3. **Pass 3 — Exceptions & Gaps**  
    → What’s missing, unclear, or inconsistent?
4. **Pass 4 — Validation with Stakeholders**  
    → “I read that policy says X — is that still true in practice?”
    

Each pass yields progressively deeper insights.

---

## 📘 7. Visual Tool: “Requirement Discovery Funnel”

``Raw Material        (Documents, Policies, Emails)                   ↓          Extracted Facts        (Rules, Data, Actors, Actions)                   ↓          Candidate Requirements        (Functional, Non-Functional)                   ↓           Validated Requirements         (Confirmed by Stakeholders)                   ↓            Approved BRD/Backlog`

🎯 _Your goal as a BA is to turn unstructured information → structured, validated needs._

---

## 🪄 8. Quick Tips While Reading Many Documents

|Tip|Benefit|
|---|---|
|Use color-coded highlights (e.g., 💛 = rule, 💙 = process, 💚 = data)|Visual separation helps pattern recognition|
|Keep a “Questions Log” as you go|Fuel for workshops later|
|Use a mind map (XMind, Miro) for cross-links|Helps when documents overlap|
|Extract all “shall/must/will” statements first|They usually hide requirements|
|Rephrase findings in “The system/user must be able to…” form|Normalizes language for BRD/Stories|
|Watch for outdated or contradictory info|Document inconsistencies early|

---

## 🧩 9. From Document Reading → Requirements Statement Template

Once you extract, standardize your phrasing:

> **Requirement ID:** RQ-001  
> **Source:** Policy Manual, Section 3.2  
> **Statement:** “The system shall validate client ID numbers against the national database before account creation.”  
> **Rationale:** Prevent fraudulent onboarding  
> **Type:** Functional Requirement  
> **Priority:** High  
> **Status:** Draft

---

### 🧠 Summary Diagram — Mental Workflow

```
Document →
Identify Purpose →
Extract Facts →
Tag as Process / Data / Rule / Actor →
Classify as BR / SR / FR / NFR / TR →
Record in Matrix →
Validate with Stakeholders →
Publish in BRD / User Stories`

```
