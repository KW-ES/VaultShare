---
type: "[[Notes]]"
related:
  - "[[Finance]]"
---
### **How FRAs (Forward Rate Agreements) Can Be Used for Hedging**

A **Forward Rate Agreement (FRA)** is a financial contract that allows two parties to lock in an interest rate for a future period. It is commonly used to **hedge interest rate risk** by fixing borrowing or lending costs in advance.

FRAs are settled in cash based on the difference between the agreed FRA rate and the actual market rate at the contract’s settlement date. No principal amount is exchanged—only the **interest differential** is settled.

---

### **Hedging Scenarios Using FRAs**

#### **1. Borrower Hedging Against Rising Interest Rates**

**Scenario:**  
A company expects to take out a **3-month loan of USD 10 million in 2 months**. It is concerned that **interest rates may rise** before the loan starts.

**Solution:**

- The company **buys a 2x5 FRA** (an FRA starting in 2 months and lasting for 3 months).
    
- This locks in a fixed interest rate for the loan period.
    
- If interest rates **rise**, the FRA compensates the company for the additional borrowing cost.
    
- If interest rates **fall**, the company pays the FRA counterparty but benefits from lower loan costs.
    

**Settlement Calculation:**

- If the FRA rate is **3.00%** and the actual market rate in 2 months is **3.50%**, the company **receives** the interest difference.
    
- If the market rate is **2.50%**, the company **pays** the difference.
    

**Outcome:** The FRA acts as insurance against rising rates.

---

#### **2. Investor Hedging Against Falling Interest Rates**

**Scenario:**  
A pension fund expects to receive **USD 50 million in 3 months**, which will be invested in a **6-month deposit**. It worries that **interest rates might fall**, reducing its investment return.

**Solution:**

- The pension fund **sells a 3x9 FRA** (starting in 3 months, lasting for 6 months).
    
- This locks in a fixed return on the future investment.
    
- If interest rates **fall**, the FRA compensates the investor.
    
- If interest rates **rise**, the investor pays the difference but benefits from higher deposit rates.
    

**Outcome:** The FRA ensures a minimum return on the investment.

---

### **Key Takeaways:**

1. **FRA Buyers Hedge Against Rising Interest Rates** (e.g., borrowers).
    
2. **FRA Sellers Hedge Against Falling Interest Rates** (e.g., investors).
    
3. **FRAs Provide Cost Certainty** by locking in future interest rates.
    
4. **Only the Interest Differential Is Settled**, making FRAs a cost-effective hedging tool.


# Own

- futures
	- long -> hedge against interest rates falling (like call option)
	- short -> hedge against interest rates rising (like put option)
- FRAs
	- long (buying fixed rate) -> hedge against rising interest rates
	- short (selling fixed rate) -> hedge against falling interest rates
- IRS
	- long (buying fixed rate) -> hedge against rising interest rates
	- short (selling fixed rate) -> hedge against falling interest rate
- IRS and FRA:
	- by buying fixed rate, if floating goes up, you've locked in a lower fixed rate (to pay)
	- by selling a fixed rate, if floating goes down, you've locked in a higher (to receive)
- Converting floating/fixed:
	- if want to convert to <mark style="background: #FFB86CA6;">fixed</mark>:
		- <mark style="background: #ADCCFFA6;">floating</mark> assets:
			- sell IRS/FRA (receive <mark style="background: #FFB86CA6;">fixed</mark> instead of receiving <mark style="background: #ADCCFFA6;">floating</mark>)
				- (receiving <mark style="background: #ADCCFFA6;">floating</mark>(asset) cancels pay <mark style="background: #ADCCFFA6;">floating</mark> (IRS))
		- floating liabilities:
			- buy IRS/FRA (pay <mark style="background: #FFB86CA6;">fixed</mark> instead of paying <mark style="background: #ADCCFFA6;">floating</mark>)
				- (pay <mark style="background: #ADCCFFA6;">floating</mark>(liability) cancels receive <mark style="background: #ADCCFFA6;">floating</mark>(IRS)))
	- if want to convert to floating:
		- <mark style="background: #FFB86CA6;">fixed</mark> assets:
			- buy IRS/FRA (receive <mark style="background: #ADCCFFA6;">floating</mark> instead of receiving <mark style="background: #FFB86CA6;">fixed</mark>)
				- (receiving <mark style="background: #FFB86CA6;">fixed</mark>(asset) cancels paying <mark style="background: #FFB86CA6;">fixed</mark>(IRS))
		- fixed liabilities:
			- sell IRS/FRA (pay <mark style="background: #ADCCFFA6;">floating</mark> instead of paying <mark style="background: #FFB86CA6;">fixed</mark>)
				- (paying <mark style="background: #FFB86CA6;">fixed</mark>(liability) cancels out receiving <mark style="background: #FFB86CA6;">fixed</mark>(IRS))
	- look at pay or receive (liability? or asset?)
		- receiving -> asset
		- paying -> liability
	- what you're getting, floating or fixed? (buy or sell?)
		- floating payments / receipts
		- fixed payments / receipts
		- *get opposite of that*
			- e.g. floating asset -> floating receipts: therefore want fixed receipts: therefore sell IRS
- hedging instruments for short term interest rate risk
	- STIR futures
	- FRAs
	- OIS
- 