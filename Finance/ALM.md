---
type: "[[Notes]]"
related:
  - "[[Finance]]"
aliases:
  - ALCO
---
- [[Hedging]]
- [[Gap Analysis]]
- [[Balance Sheet Management]]




- ALCO → Asset & Liability Committee






[[Types of Risk]]



## Purpose & Scope of ALM

### **Goal**: 
- Balance
	- profitability,
	- solvency,
	- and liquidity
- over time by managing
	- the structure
	- and risks
- of the balance sheet
	- (assets, liabilities, off-balance-sheet).

### **Risk classes in scope** [[Types of Risk]]
- **Interest rate risk in the banking book ([[IRRBB]])**:
	- earnings and value sensitivity to yield curve moves.
- **Liquidity risk**:
	- ability to fund assets and meet obligations ([[LCR]]/[[NSFR]] logic).
- **Funding & refinancing risk**:
	- tenor and stability of liabilities vs asset cashflows.
- **FX & basis risk**:
	- currency mismatches;
	- cross-currency basis.
- **Optionality/behavioural risk**: 
	- prepayments,
	- early redemptions,
	- deposit stickiness
	- & rate betas.
- **Credit migration/sector concentration**
	- (often coordinated with Credit Risk but visible to ALM through concentrations and stress).
        
### **Two lenses**
    
- **Earnings / income perspective** 
	- (short–medium horizon):
	- Net Interest Income ([[NII]]),
	- Earnings-at-Risk (EaR).
- **Value / solvency perspective**
	- (longer horizon):
	- Economic Value of Equity (EVE),
	- Economic Value-at-Risk (EVaR).

## Balance Sheet Management
![[Balance Sheet Management#Balance-Sheet Mechanics & Core Concepts]]

> [[Balance Sheet Management]]


## Key textbook metrics & approximations


> [!eg]- Key Metrics & Approximations
> - Present Value
> - Macaulay Duration
> - Modified Duration
> - DV01/PVBP
> - Duration Gap
> - EVE
> - Repricing Gap
> 
> 
> ![[IMG-20260107130926296.png]]
> 



## [[IRRBB]] (Interest Rate Risk in the Banking Book)

![[IRRBB#IRRBB in ALM]]


## Liquidity & Funding (ALM’s second pillar)

- **Structural liquidity**:
	- stability of core deposits vs wholesale funding;
	- tenor of assets.
- **Stock metrics**:
	- **[[LCR]]** (30-day stressed liquidity),
	- **[[NSFR]]** (1-year funding stability).
- **Gap profiles**:
	- cumulative maturity ladder;
	- survival horizons under name-/market-wide stress.
- **Contingent liquidity**:
	- drawdowns on lines,
	- collateral calls,
	- derivative margining.
- **Collateral management**:
	- eligibility schedules,
	- haircuts,
	- [[Rehypothecation]] limits.

> See [[Liquidity]]

## Behavioural & Optionality Models

- **NMDs (current/savings)**:
    - **Segmentation**:
	    - core vs surge;
	    - retail vs SME.
    - **Decay** / **average life**: 
	    - survival models
	    - or geometric decay.
    - **Rate beta & lag**:
	    - Δdeposit rate = beta × Δmarket rate with lag dynamics.
		    - $\Delta \text{Deposit Rate} = \beta * (\Delta \text{Market Rate with Lag Dynamics})$
- **Mortgages/loans**:
	- **prepayment models** 
		- (refi incentive, burnout, seasonality),
		- **OAS** for embedded options.
- **Term deposits**:
	- early withdrawal tendencies.
- **Implication**:
	- models feed both
		- [[NII]] and
		- EVE engines;
- *parameter governance is an ALCO responsibility.*

## Hedging

![[Hedging#Hedging in ALM]]

>See  [[Hedging]]

## FTP
![[FTP#FTP (Funds Transfer Pricing)—ALM’s operating system]]

> See [[FTP]]


## Measurement Frameworks & Models

- **Static gap**: 
	- bucketed repricing/maturity.
- **Duration/KRD**: 
	- DV01 and
	- **key-rate** decomposition
		- (2y, 5y, 10y, 30y).
- **Simulation engines**:
    - **[[NII]]**: 
	    - stochastic rate paths (e.g., Vasicek [^2]/CIR/HJM) with dynamic balance sheet assumptions. [[Balance Sheet Management]]
    - **EVE**: 
	    - shocked yield curves, optionality via OAS.
- **Risk metrics**: 
	- PVBP, 
	- ΔNII@shocks, 
	- EVE change, 
	- EaR, 
	- EVaR, and 
	- stress outcomes.
- **Model risk**: 
	- parameter uncertainty, 
	- data lineage, 
	- challenger models, 
	- back-testing, 
	- overrides.

## Governance & Process

### **ALCO** (Asset–Liability Committee): 
- approves
	- risk appetite, 
	- limits, 
	- models, 
	- [[FTP]] framework, 
	- hedges.
### **Policies & limits**:
- NII/EVE limits (absolute or as % of capital),
- PVBP/KRD limits,
- liquidity survival horizons.
- Early-warning indicators
	- (deposit outflows,
	- funding spread spikes).
### **ICAAP/ILAAP** alignment:
- capital planning &
- liquidity adequacy;
	- stress testing integration.
### **Three lines**: 
- business *(1st),* 
- ALM/risk *(2nd),* 
- audit *(3rd).*
### **Reporting cadence**:
- *monthly* ALCO packs; 
- *quarterly* stress reviews; 
- *annual* model validations.



## From [[Treasury Functions]]
![[Treasury Functions#3) ALM / IRRBB]]


[^2]: David Suriyaraachi
