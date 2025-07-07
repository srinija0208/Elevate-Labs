# 📊 Customer Segmentation using K-Means Clustering

## 🧰 Overview
This project performs **customer segmentation** using K-Means clustering on a shopping mall dataset. It analyzes customer behavior based on **Age**, **Annual Income**, and **Spending Score** to identify distinct consumer personas. 


## 🚀 Steps Involved
1. **Data Preprocessing**
   - Scaling features using `StandardScaler`
   - Optional: Removing irrelevant or noisy columns like `Gender` for clustering quality

2. **Elbow Method**
   - Plotting inertia vs. cluster count to estimate optimal `k`

3. **Silhouette Score Analysis**
   - Evaluating cluster quality across multiple `k` values

4. **Clustering with K-Means**
   - Running `KMeans` with selected `k`
   - Assigning cluster labels to data

5. **Visualization**
   - 2D scatter plots using PCA
   - Cluster-wise coloring
   - Spending and income/age analysis per group

6. **Interpretation**
   - Generating customer personas like:
     - *Affluent Minimalists*
     - *Budget-Conscious Shoppers*
     - *High-Engagement Youth*

## 📈 Dependencies
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `sklearn`

## 🧠 Key Insights
- Age and Income play pivotal roles in segmenting shoppers.
- Visualizations uncovered five clear personas, actionable for marketing and retention strategies.


