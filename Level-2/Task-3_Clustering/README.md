## Task 3 — K-Means Clustering

**Dataset:** Iris (150 records · 4 features · 3 species)  
**Tool:** Python · pandas · scikit-learn · matplotlib · seaborn · Google Colab

### What was done:
- Applied K-Means clustering with optimal K=3
- Used Elbow Method to determine optimal cluster count
- Reduced dimensions with PCA for 2D visualization (95.8% variance retained)
- Evaluated cluster quality with Silhouette Score

### Key Findings:
- **Silhouette Score: 0.459** — moderate, well-separated clusters
- **PCA variance explained: 95.8%** across 2 components
- K-Means clusters closely align with actual Iris species labels
