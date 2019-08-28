# My work as a Risk Manager
I, as a risk manager, specified risk management system requirements at work for hedge funds which were finally legalized in 2012 in South Korea. Since it's been more than seven years ago, this legacy system is *no longer used* now. Bloomberg **PORT** has replaced the system. Also, this work was done solely by me. I believe thus that it would have no adversarial effect to demenstrate my work with some screenshots of *Excel spreadsheets*, not even the real system, which I used for the specification:
- Volatility Decomposition
- VaR Analysis
- Performances and Risk Reports

**Relevant working experience**: January 2010 to February 2013 at Korea Investment Management (Seoul, KR)

This work was done in Korean, but I *translated* it to English for this posting without any further modification.

## I. Volatility Decomposition
I manually decomposes volatility (, which I take as risk) using Excel.
- Risk Sensitivity := Volatility of a single stock x Correlation of that stock with the portfolio
- Risk Contribution := Risk sensitivity of a single stock x Investment weight of that stock


### 1. Volatility Decomposition Table
Here's an example of how I specified a volatility decomposition requirement, which I passed to the internal technology team at work.

![volatility_decomposition](volatility_decomposition.png)


### 2. Volatility Decomposition by Colors
This plot efficiently summarizes the information above.

![volatility_decomposition_by_colors](volatility_decomposition_by_colors.png)



## II. VaR Analysis
We need VaR analysis in finer details for hedge funds because of various strategies within one hedge fund. So, my suggestion was to go from security-level, strategy-level and to country/sector-level analysis

![var_analysis_1](var_analysis_1.png)
![var_analysis_2](var_analysis_2.png)
![var_analysis_3](var_analysis_3.png)

#### Definitions
We intentionally use easier terms for communiations as follows:
  - Contributions is just a component VaR
  - Sensitivity is marginal VaR
  - % of Risk is percentage of sum of all contributions
  
Risk aggregation for a strategy-level analysis
  - SUM(VaR Contribution) = SUM(VaR contribution for each strategy)
  - VaR = SUM(VaR for each strategy)
  - Sensitivity = NAV-weight average(Sensitivity for each strategy)
  - Contribution = SUM(Contribution for each strategy)



## III. Performances and Risk Report
![performances_and_risk_indicators_by_strategies](performances_and_risk_indicators_by_strategies.png)
![performances_and_risk_indicators_by_strategies_2](performances_and_risk_indicators_by_strategies_2.png)
