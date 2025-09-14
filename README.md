# Weed-4class-45 Image Analysis

## Overview
Analyze the **Weed-4class-45** dataset (Lantana, Parthenium, Prickly, Siam, Negative) using **clustering** and **classification**.

---

## Dataset
- **Images:** 13,328  
- **Classes:** Lantana, Parthenium, Prickly, Siam, Negative  
- **CSV Columns:** `Filename`, `Label`, `Species`

---

## Methods

### Clustering
- **Algorithms:** KMeans, KMeans++, Bisecting KMeans, Spectral, DBSCAN, Agglomerative (single, complete, average, ward)  
- **Evaluation:** Fowlkes-Mallows Index (FMI), Silhouette Coefficient  

**Top Performers (FMI / Silhouette):**  
- DBSCAN: 0.4946 / 0.5360  
- Single Linkage: 0.4996 / 0.5335  
- Group Average: 0.4930 / 0.5263  

### Classification
- **Models & Accuracy:**  
  - SVM: **79.65%**  
  - KNN (k=7): 75.45%  
  - Decision Tree: 68.49%  
  - Naive Bayes: 22.84%  

> SVM performed best for image histogram features.

---

## Dependencies
`numpy`, `pandas`, `matplotlib`, `seaborn`, `opencv-python`, `scikit-learn`

---

## Usage
1. Convert images to grayscale and compute histograms.  
2. Apply PCA (optional) for dimensionality reduction.  
3. Train clustering or classification models.  
4. Evaluate using FMI, Silhouette score, or accuracy.  
