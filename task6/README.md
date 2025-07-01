# 🍷 Wine Classification 

This project explores classification of the Wine dataset using KNearestNeighbor. It involves data preprocessing, visualization, K-Nearest Neighbors (KNN) modeling, and interpretability through metrics and plots.

---

## 📦 Dataset
- **Source**: `sklearn.datasets.load_wine()`
- **Samples**: 178
- **Features**: 13 chemical attributes of wines
- **Target**: Multiclass (3 cultivars)

---

## 🚀 Key Tasks
- Data exploration and visualization:
  - Histograms, pairplots, and correlation heatmap

- Model training:
  - K-Nearest Neighbors (KNN) Classifier

- Model evaluation:
  - Elbow method to tune `k`
  - Confusion matrix, accuracy score

- Visualization:
  - Decision boundaries (with PCA)

---

## 📊 Results
- **Best KNN accuracy**: ~97.2% at `k = 8`

- **Clear class separability** observed in selected feature pairs and PCA-reduced plots

---

## 🛠 Libraries Used
- Python 3
- `pandas`, `numpy`, `matplotlib`, `seaborn`
- `scikit-learn`
- `mlxtend` (for visualization utilities)

---

## 🧠 Insights
- Some features show strong correlation with the target class and contribute significantly to decision boundaries.
- PCA effectively reveal class separability.
- KNN performs well even with basic preprocessing and minimal hyperparameter tuning.

