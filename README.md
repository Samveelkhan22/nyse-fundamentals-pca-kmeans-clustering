# nyse-fundamentals-pca-kmeans-clustering
This repository contains a data‐driven analysis of NYSE-listed companies’ financial fundamentals using Principal Component Analysis (PCA) and K-Means clustering. We demonstrate how to:

1. **Preprocess** company fundamentals  
2. **Reduce dimensionality** with PCA (≥ 90 % variance)  
3. **Segment** firms into clusters via K-Means  
4. **Validate** clustering stability and handle outliers  

---

## Files
- fundamentals.csv
- securities.csv
- prices.csv # optional if you include price feature
- NYSE_Fundamentals_Clustering_Analysis.ipynb

---

## Dependencies

- Python 3.8+  
- pandas  
- numpy  
- scikit-learn  
- matplotlib

---

## Usage

1. Jupyter Notebook
Open and run:
```
jupyter notebook NYSE_Fundamentals_Clustering_Analysis.ipynb
```
This notebook walks through:

- Data loading & cleaning
- Median imputation of missing fundamentals
- PCA scree plot & component selection
- K-Means elbow method & final clustering
- 2D PCA visualization & silhouette analysis
- Outlier removal (e.g. HRB) and re-clustering
  
---

## Results
- PCA reduced 6 financial metrics to 5 components, retaining ~98 % variance.
- K-Means (k = 4) produced well-separated clusters; silhouette scores ranged 0.59–0.75.
- Outlier “HRB” was isolated; removing it and re-clustering to k = 3 improved cohesion (silhouette ≈ 0.76).
- Cluster profiles highlight large blue-chips, mid-caps, cash-rich chip-makers, and outlier anomalies
