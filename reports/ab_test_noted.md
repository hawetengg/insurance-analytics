# A/B Test Notes
- Hypothesis: H0 - No difference in TotalClaims (Gauteng vs. KwaZulu-Natal)
- Data Cleaning: Removed rows with TotalPremium = 0 or TotalClaims < 0; 618,174 rows remain
- Sample Sizes: Gauteng: 249,781, KwaZulu-Natal: 111,896
- Mean TotalClaims: Gauteng: 116.2603442234579, KwaZulu-Natal: 120.883247058811
- Normality Test (Shapiro): Gauteng p-value: 4.6399440851771e-208, KwaZulu-Natal p-value: 3.4961568517774e-187 (non-normal)
- Variance Test (Levene): Not fully reported, assumed unequal
- Test: Mann-Whitney U, p-value: 9.0754157009192e-06
- Conclusion: Reject H0: Significant difference in TotalClaims
- Modeling Input: Used cleaned data for Task 4 prediction of TotalClaims