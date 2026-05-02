## Task 2 — Exploratory Data Analysis (EDA)

**Dataset:** Telco Customer Churn (churn-bigml-80.csv)  
**Records:** 2,666 rows · 21 features  
**Tool:** Python · pandas · matplotlib · seaborn · Google Colab

### What was done:
- Analyzed overall churn rate: **14.6%**
- Explored feature distributions across churned vs. non-churned customers
- Identified key churn drivers through group comparisons
- Calculated correlation matrix to detect multicollinearity

### Key Findings:
- International plan holders churn at **4x** the rate of non-holders
- Customers with **4+ service calls** show 48%+ churn probability
- Total minutes and total charges have **perfect correlation** (r ≈ 1.0)
- Voice mail plan holders show significantly lower churn tendency

### Charts:
6 visualizations covering churn distribution, plan-based churn rates,
service call impact, and feature correlations.

