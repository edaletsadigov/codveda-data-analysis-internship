## Task 1 — Churn Classification

**Dataset:** Telco Customer Churn  
- Train: churn-bigml-20.csv (667 rows · 20 features)  
- Test: churn-bigml-80.csv (2,666 rows · 20 features)  
**Tool:** Python · pandas · scikit-learn · matplotlib · seaborn · Google Colab

---

### What was done:
- Trained and compared 3 classification models: Logistic Regression, Decision Tree, Random Forest
- Applied `class_weight='balanced'` to handle class imbalance (14.6% churn rate)
- Tuned Random Forest with GridSearchCV (5-fold CV, 18 parameter combinations)
- Optimized decision threshold using Precision-Recall curve analysis

---

### Model Comparison Results:

| Model | Accuracy | Precision | Recall | F1 |
|---|---|---|---|---|
| Logistic Regression | 0.7637 | 0.3495 | 0.7242 | 0.4715 |
| Decision Tree | **0.9006** | 0.6606 | 0.6521 | **0.6563** |
| Random Forest | 0.8923 | 0.9316 | 0.2809 | 0.4317 |

**Best model by F1: Decision Tree (F1 = 0.6563)**

---

### Hyperparameter Tuning — Random Forest:

**Best parameters:** `n_estimators=200, max_depth=None, min_samples_split=10`  
**Best CV F1:** 0.6281

**Threshold optimization (default 0.50 → optimal 0.35):**

| Metric | Default (0.50) | Tuned (0.35) |
|---|---|---|
| Precision | 0.8269 | 0.6148 ↓ |
| Recall | 0.4433 | 0.6830 ↑ |
| F1-Score | 0.5772 | **0.6471** ↑ |

---

### Top 5 Features (Random Forest — Gini Importance):

| Feature | Importance |
|---|---|
| total_day_minutes | 0.2578 |
| customer_service_calls | 0.1406 |
| total_eve_minutes | 0.1243 |
| account_length | 0.0603 |
| total_night_minutes | 0.0599 |

---

### Charts:
4 visualizations: Churn Distribution, Confusion Matrices (all models),
Feature Importance, Precision-Recall Curve with threshold analysis.
