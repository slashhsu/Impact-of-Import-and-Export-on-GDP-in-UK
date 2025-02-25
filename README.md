

# Impact of Import and Export on GDP in the UK
*A Time Series Analysis Using Stata*

## Overview
This project explores the relationship between **import, export, and GDP** in the UK using time series analysis. Various econometric tests and models are employed to examine short-run and long-run relationships, particularly the **Error Correction Model (ECM)** and **Granger Causality Test**.

---

## 1. Data Visualisation
The first step in the analysis is observing the time-series trends of **GDP, import, and export**.

- **Figure 1**: Time-series plots of GDP, import, and export (both level and difference).
- The results suggest that **export and import have a positive effect on GDP**.
- A **sharp decline** is observed in 2019, likely due to the **COVID-19 pandemic**.

![Timeline of Export, Import, and GDP](https://github.com/slashhsu/Impact-of-Import-and-Export-on-GDP-in-UK/assets/137000188/dc81d006-77c1-4c5c-ba53-83c5fc9d0d93)
![Difference in Export, Import, and GDP](https://github.com/slashhsu/Impact-of-Import-and-Export-on-GDP-in-UK/assets/137000188/8b640229-5bb8-4040-b492-74b462a327e3)

---

## 2. Methodology
To ensure robust analysis, the following statistical tests and models were applied:

### (a) Pre-Analysis Tests
- ✅ **Stationarity & Autocorrelation Tests** – Check if the time series is stationary.
- ✅ **Cointegration & Lag Length Tests** – Determine the appropriate lag structure.

### (b) Econometric Model: Error Correction Model (ECM)
The ECM model is used to study the **short-run** and **long-run** relationships between GDP, import, and export.

The following equations test:
- **GDP and export**
- **GDP and import**

\[
\Delta GDP_t = \alpha + \sum \beta_i \Delta EXPORT_{t-i} + \sum \gamma_i \Delta GDP_{t-i} + \lambda ECM_{t-1} + \epsilon_t
\]

\[
\Delta GDP_t = \alpha + \sum \beta_i \Delta IMPORT_{t-i} + \sum \gamma_i \Delta GDP_{t-i} + \lambda ECM_{t-1} + \epsilon_t
\]

Where:
- \( I \) and \( L \) represent the **autoregressive order of the dependent variable**, determined by the Akaike Information Criterion (AIC).
- \( ECM \) is the error correction term, capturing the long-run equilibrium relationship.

![ECM Model](https://github.com/slashhsu/Impact-of-Import-and-Export-on-GDP-in-UK/assets/137000188/b12e5322-b155-451b-baff-67893cfef22a)
![ECM Explanation](https://github.com/slashhsu/Impact-of-Import-and-Export-on-GDP-in-UK/assets/137000188/f5409e2b-5e82-46b1-a86b-a8c7ac7ddb0c)

---

## 3. Granger Causality Test
Granger causality is used to determine whether **past values of one variable can predict future values of another**.

- ✅ If **export Granger-causes GDP**, then past export values contain useful information for forecasting GDP.
- ✅ If **import Granger-causes GDP**, it suggests that imports influence GDP movements over time.

According to **Clive Granger (1977)**, economic causality can be tested by measuring the ability of one time series to predict another.

![Granger Causality Test](https://github.com/slashhsu/Impact-of-Import-and-Export-on-GDP-in-UK/assets/137000188/0e7847f1-12de-4084-ba68-a47e54346497)

---

## 4. Key Findings
📌 **Both export and import positively impact GDP**.  
📌 The **ECM model** confirms a long-run relationship between GDP, import, and export.  
📌 **Granger causality results** suggest that changes in **exports/imports influence GDP** over time.  
📌 The **COVID-19 pandemic** caused a sharp decline in economic activity in 2019.  

---

## 5. Tools & Resources
- 🛠 **Software Used**: Stata
- 📊 **Statistical Methods**: ECM Model, Granger Causality, Cointegration Test
- 📂 **Dataset Source**: UK GDP, import, and export data

---

## 6. References
- **Granger, C.W.J.** (1977). "Investigating Causal Relations by Econometric Models and Cross-Spectral Methods." *Econometrica*  
- **Akaike, H.** (1974). "A New Look at the Statistical Model Identification." *IEEE Transactions on Automatic Control*  


6. References
Granger, C.W.J. (1977). "Investigating Causal Relations by Econometric Models and Cross-Spectral Methods." Econometrica
Akaike, H. (1974). "A New Look at the Statistical Model Identification." IEEE Transactions on Automatic Control
