---
type: "[[Notes]]"
related:
  - "[[Useful]]"
  - "[[Finance]]"
---
These are **treasury/ALM (Asset–Liability Management)** concepts, and they’re crucial when you model banking books. Let’s break them down:


## 📉 Behavioural Rate

- The **effective interest rate that customers actually earn/pay**, which may differ from the **contractual rate**.
    
- Banks apply behavioural rates when they model **deposit and loan products** where the “headline” rate doesn’t capture reality.
    

### Examples

- A current account is _contractually_ 0% interest.
    
    - But if customers leave balances there for long periods, treasury may treat part of it as if it earns a **behavioural rate** (e.g. 0.5% or linked to short-term swaps).
        
- Credit cards might show a contractual rate of 20%, but **actual behaviour** (prepayments, defaults, teaser rates) means the **behavioural yield** is lower.
    

## ⏳ Behavioural Maturity

- The **assumed effective maturity of a product based on customer behaviour**, not its legal maturity.
    
- Used in ALM to model **non-maturing deposits (NMDs)** and products with optionality.
    

### Examples

- Sight deposits (e.g. checking/current accounts) are legally payable **on demand** (maturity = overnight).
    
    - Behaviourally, customers leave balances for years.
        
    - Treasury models these as having a **behavioural maturity** of, say, 3–5 years, to match with longer-term assets.
        
- Mortgage loans may be 20 years legally, but borrowers prepay early → behavioural maturity is maybe 7–10 years.

<div style="page-break-after: always;"></div>


## 🏦 Why It Matters

- **Interest Rate Risk in the Banking Book (IRRBB):** ALM teams need behavioural assumptions to model repricing gaps and earnings at risk.
    
- **Liquidity & funding planning:** Helps decide how much “sticky” funding a bank can rely on.
    
- **Transfer Pricing:** The behavioural rate & maturity are often inputs into **Funds Transfer Pricing (FTP)** models that allocate cost of funds to businesses.
    

---

✅ In short:

- **Behavioural rate = effective interest rate implied by customer behaviour.**
    
- **Behavioural maturity = effective term/maturity implied by customer behaviour.**