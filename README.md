# Commercial Real Estate Machine Learning PD Modeling

### Model Versions
- **Version 1: The 'Legacy Benchmark'** (Weighted RF)
- **Version 2: The 'Conservative Baseline'** (Unweighted RF)
- **Version 3: The 'Engineered Champion'** (Feature-Engineered RF)

### Input Factors (Features)
The models utilize the following loan-level and market factors to estimate risk:
- **Stressed LTV**: Loan-to-Value ratio under stress scenarios.
- **DSCR**: Debt Service Coverage Ratio.
- **Occupancy**: Current physical occupancy percentage.
- **Market Stress**: Regional economic risk indicator.
- **Property Risk Flag**: Indicator for high-risk property types.
- **Sponsor Risk Score**: Qualitative score of the borrower/sponsor strength.
- **Recovery Lag Months**: Expected time to recover capital post-default.
- **Cap Rate Expansion**: Potential shift in market capitalization rates.
- **Debt Yield**: Net Operating Income divided by the total loan amount.

### Model Outputs & Performance Metrics
The analysis generates the following results:
- **Probability of Default (PD)**: The estimated likelihood of a loan defaulting (0% to 100%).
- **Brier Score**: Measures the accuracy of probabilistic predictions (lower is better).
- **AUC / Gini**: Measures the model's ability to rank loans from low to high risk.
- **KS (Kolmogorov-Smirnov)**: Measures the maximum separation between default and non-default distributions.
- **Feature Importance**: Identifies which factors (e.g., LTV vs. Sponsor Risk) most influence the final PD.
