---
type: "[[Notes]]"
related:
  - "[[Finance]]"
---

### **Caps and Floors in Interest Rate Derivatives**

**Caps and Floors** are **interest rate derivatives** used to hedge or speculate on interest rate movements. They function as **options on interest rates**, providing protection against unfavourable rate fluctuations.

---

### **1. Interest Rate Cap**

An **Interest Rate Cap** is a series of European-style **call options** (known as **caplets**) on a floating interest rate, typically **LIBOR, SOFR, or EURIBOR**.

- **Purpose:** Protects against rising interest rates.
- **Buyer’s Benefit:** If the floating rate **exceeds** the agreed cap rate, the seller pays the difference.
- **Seller’s Role:** The seller receives an upfront premium and compensates the buyer when rates rise above the cap.

#### **Example of a Cap:**

- A company with a **floating-rate loan** (e.g., LIBOR + 2%) buys a cap at **5%**.
- If LIBOR rises to **6%**, the cap seller pays the difference **(6% - 5% = 1%)** on the notional amount.
- If LIBOR stays **below 5%**, no payment is made.

---

### **2. Interest Rate Floor**

An **Interest Rate Floor** is a series of European-style **put options** (known as **floorlets**) on a floating interest rate.

- **Purpose:** Protects against falling interest rates.
- **Buyer’s Benefit:** If the floating rate **falls below** the agreed floor rate, the seller pays the difference.
- **Seller’s Role:** The seller receives an upfront premium and compensates the buyer when rates drop below the floor.

#### **Example of a Floor:**

- A bank holding **floating-rate assets** (e.g., loans earning LIBOR + 1%) buys a floor at **3%**.
- If LIBOR drops to **2%**, the floor seller pays the difference **(3% - 2% = 1%)** on the notional amount.
- If LIBOR stays **above 3%**, no payment is made.

---

### **3. Cap and Floor Combined: Interest Rate Collar**

A **collar** combines a **cap and a floor**:

- The **borrower buys a cap** (protecting against high rates).
- The **borrower sells a floor** (accepting lower rates in exchange for reduced or zero premium).
- This strategy **reduces the cost of hedging** but limits gains from falling rates.

---

### **4. Summary Table**

|Feature|Interest Rate Cap|Interest Rate Floor|
|---|---|---|
|Buyer Type|Floating-rate borrower|Floating-rate investor/lender|
|Protection|Against rising rates|Against falling rates|
|Option Type|Call options (caplets)|Put options (floorlets)|
|Buyer’s Benefit|Receives payment if rates exceed cap|Receives payment if rates fall below floor|
|Seller’s Role|Pays if rates exceed cap|Pays if rates fall below floor|
|Cost to Buyer|Pays upfront premium|Pays upfront premium|