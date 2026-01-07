---
type: "[[Notes]]"
related:
  - "[[Finance]]"
---

# ACI
## Spot Date
> The term Spot is used in many markets. In the Foreign Exchange market, **spot value date is two business days forward from deal date.** These two business days may be influenced by weekends, holidays or other non-business days involving the closure of the clearing system in the financial centres of the two currencies involved in any exchange rate quotation
> If a holiday or other closure affects this two day period the Spot value date moves forward to the next business day
[[IMG-20260107130453166.pdf#page=66&selection=179,0,190,50|ACI Textbook1, page 66]]

t + 2

> [!note] For FRA's Settlement Date = Fixing date

# ChatGPT
> [!spa] Question
> Can you explain how spot dates, forward dates, value dates, trade dates, maturity dates, settlement dates etc. all work for all instruments in the book?

Understanding **dates** like **spot dates, forward dates, value dates, trade dates, maturity dates, and settlement dates** is essential for managing transactions across financial instruments, as these govern the flow of payments and obligations in the financial markets. Below is a detailed explanation of how these dates function for various instruments, as per the ACI syllabus.

---

### 1. **Trade Date**

- **Definition**: The date on which a financial transaction (e.g., spot, forward, bond purchase) is agreed upon between counterparties.
- **Purpose**: It marks the beginning of the transaction lifecycle.
- **Application Across Instruments**:
    - **FX**: The trade date is when the parties agree to exchange currencies.
    - **Bonds**: The trade date is when the bond buyer and seller agree on the terms (e.g., price, yield).
    - **Derivatives**: The trade date initiates the derivative contract (e.g., futures or swaps).

---

### 2. **Value Date**

- **Definition**: The date when the cash or securities involved in a transaction are exchanged and settled.
- **Purpose**: Indicates when the transaction is finalized and becomes effective.
- **Application Across Instruments**:
    - **FX Spot**: The value date is typically **T+2** (two business days after the trade date).
    - **FX Forward**: The value date is agreed upon and corresponds to the forward tenor (e.g., 1 month, 3 months, etc.).
    - **Money Market Instruments**: The value date is usually **T+0**, **T+1**, or **T+2**, depending on the market convention.
    - **Bonds**: The value date is when ownership of the bond is transferred, typically **T+2**.

---

### 3. **Spot Date**

- **Definition**: The standard settlement date for a spot transaction, typically **T+2** in most financial markets.
- **Purpose**: Used as the starting point for calculating forward dates.
- **Application Across Instruments**:
    - **FX Spot**: For most currency pairs, the spot date is two business days after the trade date (T+2), except for pairs like USD/CAD and USD/TRY, which settle on **T+1**.
    - **Bonds and Equities**: Spot date aligns with the market's settlement convention (commonly T+2).
    - **Commodities**: Spot settlement depends on the commodity exchange’s rules.

---

### 4. **Forward Date**

- **Definition**: A value date beyond the spot date, agreed upon for forward transactions.
- **Purpose**: Specifies when the transaction will settle in the future.
- **Application Across Instruments**:
    - **FX Forward**: The forward date is derived from the spot date by adding the agreed tenor (e.g., 1 month, 3 months).
    - **Interest Rate Swaps**: The forward start date defines when the interest payments or obligations begin.
    - **Forward Rate Agreements (FRAs)**: The forward date is when the notional interest period begins.

---

### 5. **Maturity Date**

- **Definition**: The date on which a financial instrument expires or the principal amount is repaid.
- **Purpose**: Represents the end of the transaction lifecycle.
- **Application Across Instruments**:
    - **FX Forward/Swaps**: The maturity date is when the final exchange of currencies takes place.
    - **Bonds**: The maturity date is when the bondholder receives the principal and last coupon payment.
    - **Money Market Instruments**: Maturity corresponds to the date when the issuer repays the loan (e.g., certificates of deposit, treasury bills).
    - **Derivatives**: Futures or options contracts mature on pre-determined dates.

---

### 6. **Settlement Date**

- **Definition**: The date when the actual transfer of cash, securities, or other assets occurs.
- **Purpose**: Ensures that all parties fulfill their contractual obligations.
- **Application Across Instruments**:
    - **FX**: Settlement occurs on the value date when the agreed currencies are exchanged.
    - **Bonds and Equities**: Settlement typically occurs on **T+2** or **T+1**, depending on the market.
    - **Commodities**: Settlement happens when the physical commodity or cash equivalent is delivered.

---

### Summary of Timing Conventions:

|Instrument Type|Trade Date|Spot Date (T+X)|Value Date|Maturity Date / Final Settlement|
|---|---|---|---|---|
|**FX Spot**|T|T+2 (Standard)|T+2|N/A|
|**FX Forward**|T|T+2 (as base)|Spot Date + Forward Tenor|Forward Tenor Maturity|
|**Bonds**|T|T+2|T+2|Bond Maturity Date|
|**Money Market**|T|T+0, T+1, T+2|Tenor-Based|End of Loan/Deposit Period|
|**Derivatives (Futures)**|T|Exchange Rule|Settlement Period|Futures Expiry or Final Delivery|
|**Commodities**|T|Exchange Rule|As per Contract|Delivery or Expiry Date|

---

### Example for FX Spot and Forward:

1. **Spot Transaction**:
    
    - **Trade Date**: Monday, 1st February 2025
    - **Spot Date**: Wednesday, 3rd February 2025 (T+2)
    - **Value Date**: Same as the spot date (3rd February 2025).
2. **1-Month Forward**:
    
    - **Trade Date**: Monday, 1st February 2025
    - **Spot Date**: Wednesday, 3rd February 2025
    - **Value Date (Forward Date)**: Monday, 3rd March 2025 (1 month from the spot date).

---

> [!spa] Question
> what is a tenor?




A **tenor** refers to the length or duration of time remaining until the maturity of a financial instrument or transaction. It is used across various financial markets to describe the time period for which money is lent, borrowed, or invested.

---

### Key Features of Tenor:

1. **Time Frame**:
    
    - A tenor specifies the duration of a contract or financial instrument, such as 1 month, 3 months, 6 months, 1 year, or longer.
    - It is expressed in terms of days, months, or years.
2. **Instruments Where Tenor Applies**:
    
    - **Foreign Exchange (FX)**: For forward contracts, the tenor defines the time period beyond the spot date (e.g., 1 month forward).
    - **Money Market Instruments**: Tenor defines the duration of instruments like certificates of deposit, treasury bills, or repos.
    - **Loans & Bonds**: In loans or fixed-income securities, tenor refers to the time remaining until the principal is repaid.
    - **Derivatives**: Tenor determines the lifespan of a futures or options contract or an interest rate swap.
3. **Spot vs. Forward Tenor**:
    
    - **Spot Tenor**: Usually T+2 (two business days) in FX markets.
    - **Forward Tenor**: A specific period added to the spot date, such as 1 week, 1 month, or 1 year.
4. **Maturity and Tenor Relationship**:
    
    - The **maturity date** is the date on which the tenor ends.
    - For example, if a bond is issued with a 5-year tenor on 1st January 2025, it will mature on 1st January 2030.

---

### Examples of Tenor in Different Markets:

1. **Foreign Exchange (FX)**:
    
    - **Spot Transaction**: Has a standard tenor of 2 business days (T+2).
    - **Forward Contracts**: A tenor of 1 month, 3 months, or any agreed period beyond T+2.
2. **Money Market Instruments**:
    
    - A 90-day certificate of deposit has a tenor of 90 days from issuance.
    - A 7-day repo agreement has a tenor of 7 days.
3. **Bonds**:
    
    - A 10-year bond issued today has a tenor of 10 years, but after 2 years, its remaining tenor will be 8 years.
4. **Derivatives (Interest Rate Swaps)**:
    
    - An interest rate swap with a tenor of 5 years implies payments and settlements will occur periodically for 5 years.

---

### Why is Tenor Important?

1. **Pricing**: Tenor impacts the pricing of financial instruments. For example:
    
    - Longer tenors typically involve greater uncertainty, resulting in higher yields or premiums.
    - Shorter tenors often attract lower yields due to reduced risk.
2. **Liquidity**: Instruments with shorter tenors tend to have higher liquidity since they mature quickly.
    
3. **Risk Management**:
    
    - The tenor affects exposure to credit risk, interest rate risk, and market risk.
    - Longer tenors generally involve higher risks because they extend over a longer period.

---

> [!spa] Question 
> What are all the different dates to take into account for all the instruments? can you please make a table?

Below is a comprehensive table summarizing the **key dates** to take into account for various financial instruments, as covered in the ACI syllabus:

---

### **Key Dates Across Financial Instruments**

|**Instrument**|**Trade Date**|**Spot Date**|**Value Date**|**Maturity Date**|**Settlement Date**|**Other Dates**|
|---|---|---|---|---|---|---|
|**FX Spot**|Date of agreement between counterparties (T)|T+2 (most currencies)|T+2 (usually the same as the spot date)|N/A|When currencies are exchanged (usually T+2)|-|
|**FX Forward**|Date of agreement (T)|Derived from FX spot date (T+2)|Spot date + forward tenor (e.g., 1 month, 3 months)|Forward contract maturity date|Final exchange of currencies on forward value date|-|
|**FX Swap**|Date of agreement (T)|T+2 (for spot leg)|-|Maturity date of the forward leg|Spot leg: T+2; Forward leg: maturity of swap|-|
|**Money Market (e.g., deposits, repos)**|Date of agreement (T)|T+0, T+1, or T+2 (depending on instrument)|Start of loan period (e.g., T+1)|End of loan/deposit period (e.g., 1 month later)|Cash is delivered on value date; repaid at maturity|-|
|**Bonds**|Date of agreement (T)|T+2 (standard for bond markets)|T+2 (transfer of ownership)|Date when the principal is repaid|Same as the value date for the transaction|Coupon payment dates (semiannual/annual, etc.)|
|**Treasury Bills (T-Bills)**|Date of auction/purchase (T)|T+1 or T+2 (depending on jurisdiction)|T+1 or T+2|Maturity date (e.g., 91, 182, 364 days from issue)|Redemption at maturity date|-|
|**Forward Rate Agreements (FRAs)**|Date of agreement (T)|N/A|Start of the notional interest period|End of the notional interest period|N/A|Fixing date (2 days before start of period)|
|**Interest Rate Swaps (IRS)**|Date of agreement (T)|N/A|Start of the first interest payment period|Maturity date of the swap|N/A|Payment dates (e.g., quarterly, semiannual)|
|**Equities (Shares)**|Date of purchase/sale (T)|T+2|T+2 (ownership transfer)|N/A|Same as value date|Ex-dividend date, record date|
|**Futures Contracts**|Date contract is entered (T)|Exchange-defined (varies)|T+1 or per exchange rules|Expiry date of the contract|Physical or cash settlement at expiry|First notice date, last trading day|
|**Options**|Date contract is entered (T)|N/A|Payment of premium occurs on T|Expiry date of the option|Settlement depends on exercise date|Exercise date, settlement date, valuation date|
|**Commodities (Physical)**|Date of trade (T)|Exchange-defined|Per commodity market convention|Delivery date|Settlement at delivery date|-|
|**Commodities (Cash-settled)**|Date of trade (T)|Exchange-defined|Per exchange rules|Expiry date|Cash settlement at expiry|-|
|**Repos (Repurchase Agreements)**|Date of agreement (T)|T+0, T+1|Cash delivery occurs at start date|End date (when collateral is returned)|Repurchase occurs at maturity|-|
|**Certificates of Deposit (CDs)**|Date of issuance (T)|N/A|Issue date (start of deposit)|Maturity date|N/A|-|
|**Mortgage-Backed Securities (MBS)**|Date of trade (T)|T+2 (standard for bond markets)|T+2|Final maturity depends on prepayments|Settlement happens at T+2 or maturity|Monthly payment dates (cash flow schedule)|

---

### **Explanation of Key Dates**

1. **Trade Date (T)**:
    
    - The date on which the transaction is agreed between parties.
    - Applies universally to all instruments.
2. **Spot Date**:
    
    - The standard settlement date for spot transactions, typically T+2 in most markets.
    - Not relevant for all instruments (e.g., options or FRAs).
3. **Value Date**:
    
    - The date when cash flows, securities, or commodities are exchanged.
    - For FX and bonds, this typically coincides with the spot date or forward date.
4. **Maturity Date**:
    
    - The end date of the instrument or contract, when principal or final obligations are settled.
    - Applies to bonds, loans, forwards, swaps, and other instruments.
5. **Settlement Date**:
    
    - The date on which the actual transfer of assets (e.g., cash or securities) occurs.
    - For spot transactions, this is typically the same as the value date.
6. **Other Dates**:
    
    - **Coupon Payment Dates**: For bonds, these are pre-specified dates on which interest payments are made.
    - **Expiry Date**: The final date for options or futures contracts.
    - **Fixing Date**: For FRAs or swaps, the date when the interest rate is determined.

---

> [!spa] Question
> What is deal date?


The **deal date** is the same as the **trade date**—it refers to the date on which a financial transaction is agreed upon between two counterparties. This is the starting point of the transaction lifecycle, marking the day when the terms of the trade (e.g., price, amount, tenor, value date, etc.) are finalized.

---

### **Key Features of the Deal Date**:

1. **Initiation of the Trade**:
    
    - The deal date is the day on which the parties enter into an agreement for a transaction, such as an FX trade, bond purchase, money market deposit, or derivative contract.
2. **Time of Agreement**:
    
    - The actual time of the deal within the day is important for determining whether it falls into the current business day or rolls over to the next (based on market cutoff times).
3. **Basis for Other Dates**:
    
    - Other dates, such as the **spot date**, **value date**, and **maturity date**, are calculated based on the deal date.

---

### **Application of Deal Date Across Instruments**:

|**Instrument**|**Deal Date (Trade Date)**|**How It Relates to Other Dates**|
|---|---|---|
|**FX Spot**|Date of agreement (T)|Spot date is typically T+2; value date matches spot date.|
|**FX Forward**|Date of agreement (T)|Forward value date is calculated from spot date + forward tenor.|
|**Bonds**|Date of agreement (T)|Settlement date is typically T+2 for most bond markets.|
|**Money Market Deposits**|Date of agreement (T)|Value date is T+0, T+1, or T+2, depending on the market.|
|**Futures**|Date of entering the contract (T)|Expiry or settlement date is predefined by the exchange.|
|**Options**|Date of agreement (T)|Premium is settled on T (for OTC trades) or per exchange rules.|
|**Swaps**|Date of agreement (T)|The start of the swap (value date) is often T+2 or later.|

---

### **Why is the Deal Date Important?**

- It serves as the **reference point** for calculating other dates, such as the spot date, value date, and maturity date.
- It is a **record-keeping marker**, as financial transactions must be recorded based on the date the trade is struck.
- It determines **cutoff times** for a transaction, as trades executed after a market's cutoff time are assigned the next business day as the deal date.

---

### **Example**:

#### FX Spot Trade:

- **Deal Date**: Monday, 5th February 2025.
- **Spot Date**: Wednesday, 7th February 2025 (T+2 from the deal date).
- **Value Date**: Same as the spot date: 7th February 2025.

