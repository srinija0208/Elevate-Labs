
Titanic Dataset – Data Preprocessing Pipeline

📌 Overview

This project involves preprocessing the classic Titanic dataset from Kaggle. The goal was to prepare the data for machine learning by addressing missing values, encoding categorical features, handling outliers, and scaling the dataset.

🗂️ Dataset

Source: Kaggle Titanic

Target Variable: Survived (0 = No, 1 = Yes)

Rows & Columns: 891 rows × 12 columns (after dropping irrelevant features)

🧰 Tools & Libraries Used

Python 3.x
pandas
numpy
seaborn
matplotlib
scikit-learn

🔄 Preprocessing Steps

1. Exploratory Data Analysis (EDA)
Inspected data types and missing values
Reviewed class balance of the target variable
Used visualizations like countplots, boxplots, and histograms

2. Handling Missing Values
Used median imputation for numerical features (Age, Fare)
Used mode imputation for categorical features (Embarked)

3. Outlier Detection & Removal
Applied the IQR (Interquartile Range) method to identify and remove outliers in numerical columns like Age and Fare
Visualized outliers using boxplots

4. Encoding Categorical Variables
Used Label Encoding for binary categorical features (e.g., Sex)
Applied One-Hot Encoding for non-binary features like Embarked

5. Feature Scaling
Applied Standardization using StandardScaler to normalize numerical features (e.g., Age, Fare)

✅ Output

Final cleaned dataset is ready for ML classification models

Handled:

- All missing values
  
- Outliers using robust IQR method
  
- Categorical encoding
  
- Feature scaling using StandardScaler
