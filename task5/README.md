# 🏦 Loan Approval Prediction - ML Pipeline Project

This project builds an end-to-end machine learning pipeline to predict loan approval status based on applicant demographics, income, credit history, and other financial features.

## 🚀 Project Objectives

1. Train a **Decision Tree Classifier** and visualize the tree structure.
2. Analyze **overfitting/underfitting** using learning curves and control model complexity.
3. Train a **Random Forest Classifier** and compare its performance.
4. Interpret model behavior via **feature importances** and visualizations.
5. Evaluate both models using **cross-validation** and key classification metrics.

## 🧠 Dataset Overview

- Features: ApplicantIncome, CoapplicantIncome, LoanAmount, Loan_Amount_Term, Credit_History, Gender, Education, Property_Area, etc.
- Target: `Loan_Status` (Y = approved, N = rejected)
- Includes both categorical and numerical features

## 🛠️ Modeling Steps

- **Preprocessing**: Handled using `ColumnTransformer` with:
  - `SimpleImputer`, `StandardScaler` for numeric
  - `OneHotEncoder` for categorical
- **Pipelines**: Used `Pipeline()` to streamline transformations + modeling
- **Models**:
  - `DecisionTreeClassifier` with `GridSearchCV` for depth tuning
  - `RandomForestClassifier` with hyperparameter tuning
- **Evaluation**:
  - `cross_val_score`, `cross_validate` with accuracy, precision, recall, and F1
  - Learning curves to diagnose bias vs variance
  - Visualized feature importances and data distributions

## 📈 Key Findings

- **Random Forest** significantly outperformed Decision Tree:
  - F1 score improved from ~65% to ~75%
  - Validation accuracy increased from ~55% to ~64%
- **Credit History**, **Income**, and **LoanAmount** were top predictive features
- Overfitting was visible in Decision Tree but addressed via pruning and ensembles
- EDA revealed skewed distributions and highlighted categorical approval trends (e.g., graduates had higher approval)

## 📊 Visuals Included

- Correlation heatmap
- Learning curves
- Feature importances (side-by-side)
- Pair plots & categorical approval bar charts

## 🧩 Future Ideas

- Try XGBoost or logistic regression for comparison
- Apply threshold tuning or cost-sensitive learning
- Build a Streamlit dashboard for deployment

---

### ✅ Tools Used

`Python`, `pandas`, `matplotlib`, `seaborn`, `scikit-learn`

---

This was a hands-on ML journey—from raw data wrangling to model tuning and interpretation.  
