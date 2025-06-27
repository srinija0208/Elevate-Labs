# ❤️ Heart Disease Prediction using Logistic Regression

This project involves predicting the presence of heart disease using the UCI Heart Disease dataset. The goal is to explore the data, build a logistic regression model, and evaluate it using classification metrics. Threshold tuning was also applied to balance recall and precision for medical relevance.

---

## 📊 Dataset Overview

- **Target Variable**: `target` (1 = presence of heart disease, 0 = absence)
- **Features**: 13 clinical features including age, sex, chest pain type, fasting blood sugar, ECG results, max heart rate, ST depression, number of major vessels, and thalassemia type.

---

## ✅ Key Insights

### 📌 Categorical Feature Insights:
- **Sex**: Males are more likely to have heart disease in this dataset.
- **Fasting Blood Sugar**: Surprisingly, more heart disease cases occur in patients with normal fasting blood sugar.
- **Exercise-Induced Angina**: Absence is more frequent in those with disease.
- **Chest Pain Type**: 'Atypical' and 'Non-anginal' types are common in heart disease cases.
- **Resting ECG**: ST-T abnormalities are linked to heart disease.
- **ST Slope**: 'Flat' and 'downsloping' slopes correlate with disease presence.
- **Thalassemia**: 'Fixed' and 'reversible' defects are strongly associated with heart disease.

### 📌 Numerical Feature Insights:
- `age`, `resting_blood_pressure`, and `cholesterol` are slightly right-skewed.
- `max_heart_rate` is roughly normally distributed.
- `st_depression` and `major_vessels` are heavily skewed and may require transformation or scaling.
- The heatmap reveals **moderate positive correlations** between `age`, `major_vessels`, and `st_depression`.

---

## ⚙️ Model Performance (Logistic Regression)

- **Accuracy**: ~84%
- **Precision**: ~81%
- **Recall**: ~86%
- **F1-score**: ~83%

✅ After **threshold tuning** (from 0.5 to 0.4), recall improved with minimal impact on precision — making the model more suitable for real-world medical use.

---

## 🧠 Conclusion

Logistic regression, combined with proper preprocessing and threshold tuning, gives strong performance in predicting heart disease. Emphasis was placed on **recall** due to the critical need to avoid missing true positive cases in healthcare applications.

---

## 📚 References

- UCI Heart Disease Dataset: https://archive.ics.uci.edu/ml/datasets/Heart+Disease
- Scikit-learn, Seaborn, Pandas, Matplotlib
