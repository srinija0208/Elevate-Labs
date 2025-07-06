# Placement Prediction Using Machine Learning

This project predicts student placement status (Placed or Not Placed) based on academic performance, educational background, and other categorical factors using various machine learning models.

## 📂 Dataset
The dataset includes student-level features like:
- Academic scores (SSC, HSC, Degree, MBA)
- Educational background (boards, stream, specialization)
- Work experience
- Placement status (target)

## Techniques Used
- Exploratory Data Analysis (EDA)
- Handling missing values and outliers
- Label Encoding & One-Hot Encoding
- Feature Scaling (StandardScaler)
- PCA for dimensionality reduction
- Model Training: SVC
- Hyperparameter tuning using GridSearchCV
- Evaluation using accuracy, precision, recall, F1-score, and confusion matrix

## 🧠 Best Model Performance (SVM with PCA)
- **Accuracy:** 88.3%
- **Precision:** 90.6%
- **Recall:** 93.5%

## 📊 Visualizations
- Boxplots, countplots, correlation heatmap
- PCA decision boundaries
- Confusion matrix and classification report

## 💡 Conclusion
The SVM model with PCA performed best in predicting placements. Academic consistency and MBA scores had strong influence on placement chances.



