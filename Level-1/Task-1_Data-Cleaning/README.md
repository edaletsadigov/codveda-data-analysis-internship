## Task 1 — Data Cleaning

**Dataset:** Telco Customer Churn (churn-bigml-80.csv)  
**Input:** 2,666 rows · 21 columns  
**Output:** 2,666 rows · 20 columns (cleaned)

### What was done:
- Removed `phone number` column (non-analytical identifier)
- Converted boolean columns (`yes/no`) to binary (1/0)
- Verified: zero null values, no duplicates
- Standardized column names to snake_case

### Output file:
`churn_cleaned.csv`
