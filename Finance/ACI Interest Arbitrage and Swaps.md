---
type: "[[Study Notes]]"
thread: "[[Grad Training Main]]"
module: "[[ACI]]"
related:
  - "[[Finance]]"
---
You are overlent in 3 months EUR deposit. You need to square the position using the USD deposit market and a EUR/USD interest arbitrage swap. You are quoted the following EUR/USD swap rates. Which would be the best rate to use?

![[Pasted image 20250326154024.png]]

### **Understanding the Question: Interest Arbitrage Swap and Choosing the Correct Rate**

This question involves **closing (squaring) an over-lent EUR position** using a **EUR/USD interest arbitrage swap**. The key is to understand:

1. **What it means to be overlent in EUR.**
    
2. **How to use a EUR/USD swap to square the position.**
    
3. **How to select the correct bid/offer rate from the swap quote.**
    

---

## **Step 1: Understanding the Position – Overlent in EUR**

- Being **overlent in EUR** means you have **excess EUR deposits** that you need to convert into USD deposits.
    
- To square (eliminate) the position, you need to **sell EUR and buy USD now** (near leg) and **buy EUR and sell USD later** (far leg).
    
- This is done using a **EUR/USD interest arbitrage swap**, which allows you to temporarily convert your EUR deposit into a USD deposit.
    

---

## **Step 2: How the EUR/USD Swap Works**

A swap quote consists of **forward points** (e.g., **12-7**), which adjust the spot rate to determine the forward rate.

- **The bid (12 points):** The price at which the market maker is willing to **buy EUR forward** (i.e., when you sell EUR forward).
    
- **The offer (7 points):** The price at which the market maker is willing to **sell EUR forward** (i.e., when you buy EUR forward).
    

Since you need to **sell EUR now (buy USD) and later reverse it (buy EUR, sell USD)**, you must choose the correct side of the swap quote.

---

## **Step 3: Choosing the Correct Swap Rate**

### **Near Leg: Selling EUR and Buying USD**

- When selling EUR **now**, you use the market **bid price** (since the dealer buys EUR from you).
    
- From the swap quote **12-7**, the bid price is **12 points**.
    

### **Far Leg: Buying EUR and Selling USD**

- When buying EUR **later**, you use the **offer price** (since the dealer sells EUR to you).
    
- From the swap quote **12-7**, the offer price is **7 points**.
    

Thus, the correct answer is **12-7**, which corresponds to **option D** in the question.

---

## **Step 4: Key Rule for Choosing Swap Rates in Arbitrage Swaps**

When dealing with swaps:

- **Selling the base currency (EUR) now and buying it back later:** Use **bid price first, then offer price**.
    
- **Buying the base currency (EUR) now and selling it later:** Use **offer price first, then bid price**.
    

---

### **Final Answer and Explanation**

The correct choice is **D (12-7)** because:  
✅ **Sell EUR now → Use the bid side (12 points)**  
✅ **Buy EUR later → Use the offer side (7 points)**  
✅ **This minimizes the loss due to the spread and is the most favorable quote for the trader**