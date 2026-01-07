---
type: "[[Notes]]"
related:
  - "[[Finance]]"
  - "[[Treasury]]"
  - "[[ALM]]"
  - "[[Basel Regulations]]"
document:
  - "[[IMG-20260107130937768.pdf]]"
---


# Core Treasury Functions
> What Treasury Does

## 1) Liquidity management
> — always have cash when/where needed

- **What it means:**
	- Make sure the bank can pay everything due today and tomorrow:
		- client withdrawals,
		- settlements,
		- payroll,
		- margin calls,
		- taxes. 
- **How it works:**
	- Keep a rolling cash-flow ladder
		- (morning/noon/close; T+0 to T+7),
	- maintain a buffer,
	- and line up borrowing/investing to cover dips.

> [!eg]- Example
> 
> ![[IMG-20260107130938370.png]]



## 2) Funding the balance sheet
> — pick the right mix of money

- **What it means:**
	- Decide how much to fund
		- O/N vs term;
		- secured vs unsecured;
		- and when to issue CP/MTN.
- **How it works:**
	- Blend for cost + resilience.
	- Short money is flexible but can reprice;
	- term money fixes cost;
	- secured money is cheaper but uses collateral.

> [!eg]- Example
> 
> ![[IMG-20260107130938852.png]]

## 3) ALM / IRRBB

> — line up earnings vs funding when rates move

- **What it means:**
	- The bank often l*ends long and borrows short*.
		- If rates jump,
			- funding gets expensive before loan income catches up.
- **How it works:**
	- Measure repricing gaps,
	- set limits,
	- and use interest-rate swaps (IRS)
	- so income and costs move together.


> [!eg]- Example (NII Sensitivity)
> 
> ![[IMG-20260107130939330.png]]


## 4) FX & currency management
> — get the right currency, not just cash

- **What it means:** 
	- Ensure money is
		- in the right currency
		- and on time;
	- manage net-open-position (NOP) limits.
- **How it works**:
	- Use FX swaps/CCS to fund books,
	- and a roll calendar to avoid **bunching**.


> [!eg]- Example (NOP + Roll)
> 
> 
> ![[IMG-20260107130939834.png]]



## 5) Collateral & securities finance
> — turn assets into cheaper cash (and fees)

- **What it means:**
	- Borrow cheaper
		- by pledging high-quality collateral (repo) 
	- and earn fees
		- by lending securities.
- **How it works:**
	- Eligibility lists and haircuts define what can be pledged;
	- margining keeps exposure covered as prices move.


> [!eg]- Example (Repo w/ Margin call)
> 
> 
> ![[IMG-20260107130940325.png]]


## 6) Payments & settlements oversight

> — make money actually move

- **What it means:**
	- Ensure wires/settlements are
		- on time
		- with clean controls.
- **How it works:**
	- Maintain accurate SSIs,
	- watch cut-offs,
	- target high STP
		- with clear repair workflows.


> [!eg]- Example
> 
> 
> ![[IMG-20260107130940758.png]]

## 7) Transfer pricing (FTP)
> — set the internal price of money

- **What it means:**
	- Business units pay/receive an internal rate
		- so product pricing reflects *the true cost of funds*.
- **How it works**: 
	- For each currency/tenor
		- publish FTP = reference curve + liquidity premium (and any policy spreads).
		- *Charge at matched maturity.*

$FTP = Reference Curve + ( Liquidity Premium + Policy Spreads)$


> [!eg]- Example
> 
> 
> ![[IMG-20260107130941207.png]]

## 8) Regulatory & reporting touchpoints
> — show the bank is liquid and safe

- **What it means:**
	- Produce liquidity/encumbrance metrics
		- e.g.
			- LCR / 
			- NSFR
		- and stress results on time,
			- with reconciled data.
- **How it works**:
	- Aggregate balances/cashflows,
	- apply rulebooks,
	- publish packs to management/regulators.




> [!eg]- Example (LCR & NSFR & Emcumbrance)
> 
> ![[IMG-20260107130941629.png]]
> ![[IMG-20260107130942065.png]]
