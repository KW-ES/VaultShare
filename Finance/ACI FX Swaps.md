---
type: "[[Study Notes]]"
thread: "[[Grad Training Main]]"
module: "[[ACI]]"
related:
  - "[[Finance]]"
---


### **Understanding How to Choose Prices in FX and Swap Transactions**

To answer these types of questions correctly, you need to clearly understand **bid/offer quotes, how swap quotes work, and how to determine the correct price to use when buying or selling a currency**. Below is a structured explanation of how to approach such questions.

---

## **1. Understanding Bid/Offer Quotes in FX Transactions**

A **bid/offer (bid/ask) quote** in FX represents two prices:

- **Bid price:** The price at which the dealer (market maker) is willing to **buy** the base currency.
    
- **Offer (Ask) price:** The price at which the dealer is willing to **sell** the base currency.
    

### **How to Choose Prices in Buy/Sell Transactions**

- If **you are buying the base currency**, you **pay the offer (higher price)**.
    
- If **you are selling the base currency**, you **receive the bid (lower price)**.
    

**Example (EUR/USD quote: 1.1050 - 1.1055):**

- If you **buy EUR**, you pay **1.1055** (offer).
    
- If you **sell EUR**, you receive **1.1050** (bid).
    

---

## **2. How Swap Quotes Work in FX Swaps**

An **FX swap** consists of two transactions:

1. **You sell one currency and buy another now (near leg)**
    
2. **You reverse the trade at a future date (far leg)**
    

Swap quotes are given as **forward points**, which are added to or subtracted from the spot rate.

### **Understanding a Swap Quote (Example: EUR/GBP 6-month swap 46-50):**

This means:

- **Bid (46 points):** If you **want to sell EUR forward**, you get 46 points added to the spot rate.
    
- **Offer (50 points):** If you **want to buy EUR forward**, you must pay 50 points over the spot rate.
    

Thus:

- If you **buy EUR (sell GBP) forward**, you use **50** (the offer price).
    
- If you **sell EUR (buy GBP) forward**, you use **46** (the bid price).
    

---

## **3. How to Approach a Swap Trade (Sell X Now, Buy Y Later)**

1. **Initial Transaction (Near Leg)**
    
    - If you **buy GBP and sell EUR now**, you take the **offer price** of the swap quote.
        
    - If you **sell GBP and buy EUR now**, you take the **bid price** of the swap quote.
        
2. **Closing the Position (Far Leg)**
    
    - When you **reverse the trade**, you use the **opposite side** of the new bid/offer quote at the later time.
        

**Applying to the Given Question (EUR/GBP 6-month swap 46-50, later 52-56):**

- You **buy EUR and sell GBP at 50** (offer).
    
- Later, the market moves to **52-56**.
    
- When you **close the trade (sell EUR and buy GBP back)**, you do it at **52** (bid).
    
- The difference is **52 - 50 = 2 points profit**.
    

---

## **4. General Tricks & Hints to Solve Swap Questions**

1. **Always identify what you are buying and selling** (base currency vs. quote currency).
    
2. **Choose the correct bid or offer price based on whether you are buying or selling.**
    
    - If buying the base currency → Use **offer**.
        
    - If selling the base currency → Use **bid**.
        
3. **When closing a position, always use the opposite side of the market.**
    
4. **Forward points are added to the spot rate if in premium, subtracted if in discount.**
    
5. **Keep track of the direction of the trade** – whether you are profiting from a widening or narrowing of swap points.
    

---

### **Conclusion**

- **FX swaps involve two legs: an initial transaction and a reversal later.**
    
- **Bid/Offer spreads determine the price you get when buying or selling a currency.**
    
- **To close a position, you take the opposite side of the new quote.**
    
- **By carefully selecting the right bid or offer price, you can determine profits or losses.**
    

Would you like more examples or a step-by-step walkthrough of a different swap scenario?