## Task 1 — Regression Analysis

**Dataset:** Boston Housing (house_Prediction.csv)  
**Tool:** Python · pandas · scikit-learn · matplotlib · Google Colab

### What was done:
- Applied Linear Regression as baseline model
- Upgraded to Polynomial Regression (degree=2) for non-linear relationships
- Evaluated model performance with R² and MSE metrics
- Visualized actual vs. predicted values

### Results:
| Model | R² Score |
|-------|----------|
| Linear Regression | < 0.8056 |
| Polynomial Regression (degree=2) | **0.8056** |

### Key Insight:
Polynomial transformation captured non-linear relationships between
housing features and price, improving predictive accuracy over
the linear baseline.
