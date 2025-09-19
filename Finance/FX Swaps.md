---
type: "[[Notes]]"
related:
  - "[[Finance]]"
---

In an **FX swap**, a market maker quotes a **bid** and an **offer** for the swap points (the forward points added to or subtracted from the spot rate). The market maker's role involves both buying and selling currencies at different points in time.

Here's how it works:

## **Understanding the Market Maker's Position**

- The market maker **buys at the bid price** and **sells at the offer price** (just like in a regular FX trade).
- In an **FX swap**, the market maker is simultaneously entering into two transactions:
    1. **A spot transaction (T+2 settlement in most cases)**
    2. **A forward transaction (reversing the spot trade at a future date)**

## **Bid and Offer in FX Swaps**

1. **On the bid side:**
    - The market maker **buys the near leg (spot or short-term date)**
    - Simultaneously **sells the far leg (forward date)**
    - The bid price represents the swap points at which the market maker is willing to do this.
2. **On the offer side:**
    - The market maker **sells the near leg**
    - Simultaneously **buys the far leg**
    - The offer price represents the swap points at which the market maker is willing to do this.


| Side  | Near Leg (spot / short-term date) | Far Leg (Future / Forward Date) |
| ----- | --------------------------------- | ------------------------------- |
| Bid   | Buy                               | Sell                            |
| Offer | Sell                              | Buy                             |

### **Example Scenario**

Let’s say the spot EUR/USD rate is **1.1000** and the swap points for a one-month swap are quoted as **5/7** (meaning bid = 5, offer = 7).

- If a customer wants to **buy EUR forward**, they will pay the **offer** (7 swap points), meaning their forward rate will be **1.1007**.
- If a customer wants to **sell EUR forward**, they will receive the **bid** (5 swap points), meaning their forward rate will be **1.1005**.

Thus, as a **market maker**, you:

- **Buy at the bid (5 swap points)**
- **Sell at the offer (7 swap points)**