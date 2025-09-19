---
type: "[[Notes]]"
related:
  - "[[Finance]]"
---


### **General Rule for Sensitivities**

A **sensitivity** quantifies the response of an **output** (dependent variable) to changes in an **input** (independent variable).

![[Pasted image 20250320152928.png]]

This is the basic formula that applies across different domains.

- If small changes in the input lead to **large** changes in output, sensitivity is **high**.
- If small changes in the input lead to **small** changes in output, sensitivity is **low**.
- If the output does not change at all when the input changes, sensitivity is **zero**.

---

### **Types of Sensitivities**

1. **Absolute Sensitivity:** Measures the raw change.
    ![[Pasted image 20250320152950.png]]
2. **Relative Sensitivity (Elasticity):** Measures sensitivity as a percentage change.
![[Pasted image 20250320153005.png]]
    
3. **Gradient-Based Sensitivity:** In calculus, the derivative ![[Pasted image 20250320153021.png]] gives the local rate of sensitivity.
    
    - Used in **machine learning** (how much a small weight change affects loss).
    - Used in **physics** (how a force changes with position).
4. **Multi-Factor Sensitivity:** Sensitivity when multiple inputs affect an output.
    
    - In finance, the **Greeks** measure sensitivities:
        - **Delta** (Δ\DeltaΔ) measures price sensitivity to an asset.
        - **Gamma** measures how delta changes.
        - **Theta** measures sensitivity to time.

---

### **How to Work with Sensitivities**

1. **Identify the Key Variable and Input-Output Relationship**
    
    - What are you measuring? (e.g., speed vs. fuel efficiency)
    - What influences it? (e.g., temperature, time, external forces)
2. **Choose the Right Sensitivity Measure**
    
    - Derivatives? (Continuous data)
    - Ratios? (Discrete or relative change)
    - Experimental Observation? (If no mathematical model exists)
3. **Test and Analyse Sensitivity**
    
    - **Plot changes** (Graph it!)
    - **Simulate variations** (Monte Carlo simulations in finance)
    - **Perform local vs. global sensitivity analysis** (Does the relationship hold for all values?)
4. **Optimize or Control Based on Sensitivity**
    
    - If sensitivity is high, small adjustments matter → precise control is needed.
    - If sensitivity is low, large changes are needed to make an impact.

---

### **Example Applications**

- **Engineering:** Material stress sensitivity to force.
- **Finance:** Option price sensitivity to interest rates.
- **Climate Science:** Temperature sensitivity to greenhouse gas emissions.
- **Biology:** Drug sensitivity in different patients.