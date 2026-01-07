---
aliases:
  - Bond Durations
  - Macaulay Durations
  - Duration Calculations
type: "[[Notes]]"
related:
  - "[[Finance]]"
---
### **Duration: Definition, Pricing, Reporting, and Sensitivity**

**Duration** is a key measure in fixed income analysis that quantifies the *sensitivity* of a bond's price to interest rate changes. It helps investors and risk managers assess interest rate risk and manage bond portfolios effectively.

### **1. Understanding Duration**

Duration is a measure of the **weighted average time** an investor needs to wait to receive a bond’s cash flows (coupons + principal). It also serves as an **approximate measure of price sensitivity to interest rate changes**.

There are several types of duration:

- **Macaulay Duration** – Measures the weighted average time to receive cash flows.
- **Modified Duration** – Measures price sensitivity to changes in yield.
- **Effective Duration** – Accounts for bonds with embedded options.

---

### **2. Macaulay Duration**

**Macaulay Duration (Dm)** represents the **weighted average time (in years) until a bondholder receives cash flows**. It is calculated as:

![[IMG-20260107130930908.png]]

#### **Key Interpretation of Macaulay Duration**

- If a bond has a **Macaulay Duration of 5 years**, this means the weighted average time to recover the initial investment is **5 years**.
- <mark style="background: #FFF3A3A6;">It is primarily useful for matching assets and liabilities in fixed income portfolios.</mark>
	- *Think mismatching and gap analysis in ACI*: [[IMG-20260107130453166.pdf#page=449&selection=72,0,72,15|ACI Textbook1, page 449]]


---

### **3. Modified Duration (Price Sensitivity to Yield)**

**Modified Duration (`D*m`​)** measures the percentage change in a bond’s price for a **1% change in yield** and is *derived from* Macaulay Duration (see Dm in the formula)aa:

![[IMG-20260107130931198.png]]
#### **How Modified Duration Works in Pricing**

The bond price change is estimated using:

![[IMG-20260107130931496.png]]
**Example:**  
If a bond has:

- **Price = $1,000**
- **Modified Duration = 6**
- **Yield increases by 1% (0.01 in decimal)**

Then:

![[IMG-20260107130931786.png]]

New Price:

![[IMG-20260107130932151.png]]

Thus, the bond price falls to **$940** when the yield rises by **1%**.

---

### **4. Effective Duration (For Bonds with Embedded Options)**

For callable or putable bonds, the cash flows are **uncertain** due to optionality. **Effective duration** measures sensitivity to interest rate changes by incorporating potential cash flow changes. It is estimated using a pricing model:

![[IMG-20260107130932462.png]]

---

### **5. Reporting and Risk Management with Duration**

#### **(a) Duration in Financial Reports**

- **Used in risk disclosures** for bond portfolios in financial institutions.
- Reported as a **weighted average duration** for diversified portfolios.

#### **(b) Duration for Asset-Liability Management (ALM)**

- Banks and pension funds use **duration matching** to minimize interest rate risk.
- **Duration gap** measures mismatch between asset and liability durations.

#### **(c) Interest Rate Sensitivity in Risk Management**

- **Regulators (Basel III)** require banks to monitor duration risk.
- **Hedging strategies** use duration-based derivatives (e.g., interest rate swaps).

---

### **6. Summary of Key Duration Concepts**

|**Type of Duration**|**Definition**|**Usage**|
|---|---|---|
|**Macaulay Duration**|Weighted average time to receive bond cash flows.|Used in ALM and immunization strategies.|
|**Modified Duration**|Price sensitivity to small yield changes.|Used for estimating bond price movements.|
|**Effective Duration**|Duration adjusted for bonds with embedded options.|Used for callable/putable bonds.|

### **Conclusion**

- **Macaulay Duration** helps measure time-weighted cash flows.
- **Modified Duration** provides an estimate of price sensitivity.
- **Effective Duration** is used when bonds have optionality.
- **Duration is essential for pricing, reporting, and interest rate risk management.**

## From ACI
- Duration is a NPV of cash flows which are time weighted.
- Duration can be used to rank bonds’ price sensitivity to changes in interest rates.
	-  It can be used as a tool for managing interest rate risk.
- Duration is the weighted average cash flow of a bond, where the present values of the cash flows serve as the weights adjusted by time. Duration is the future point in TIME at which, on average, the investor has received exactly half of the original investment in PV terms.
- Modified Duration:
	- defined as “the percentage change in a bond’s dirty price for a 1 p.c. change in yield”
	-  Modified Duration is an estimate of the bond’s price sensitivity to changes in yield.
	- Acts as a multiplier
	- "Price acceleration or deceleration"
- Effective duration:
	- used instead of modified duration because the presence of prepayments changes the level of cash flow (seldom the case in wholesale market transactions). 
	- *Modified duration assumes constant cash flow.*
	- As market yields rise, effective duration lengthens and price declines accelerate compared with what is implied by the instrument’s modified duration. The price increase associated with a given decline in interest rates is smaller than the price decrease for the same size interest rate increase.
- Negative and Positive (Duration // Convexity)
	- [[IMG-20260107130453166.pdf#page=452&selection=81,0,83,0|ACI Textbook1, page 452]]