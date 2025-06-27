# 🏠 California Housing Price Prediction

This project uses the California Housing dataset to build a regression model that predicts median house values based on various housing and geographic features.

## 📊 Dataset
- **Source**: Scikit-learn's `fetch_california_housing()`
- **Target Variable**: `MedHouseVal` (Median House Value)
- **Features**:
  - Median Income
  - House Age
  - Average Rooms
  - Average Bedrooms
  - Population
  - Average Occupancy
  - Latitude & Longitude

## ⚙️ Preprocessing
- Checked for missing values (none)
- Winsorized selected numerical features to handle outliers
- Standardized features using `StandardScaler`

## Model
- **Algorithm**: Linear Regression
- **Train-Test Split**: 80-20

## Evaluation Metrics
- **Mean Absolute Error (MAE)**: ~0.533
- **Mean Squared Error (MSE)**: ~0.556
- **R² Score**: ~0.576

## 📌 Interpretation
- The model explains ~57.6% of the variance in house values.
- Median Income had the strongest positive impact on house price.
- Latitude and Longitude had negative effects, suggesting location significantly affects value.

## Limitations
- Linear regression underperforms on non-linear relationships.
- Better performance may be possible with tree-based or ensemble models.


## Dependencies
- Python
- pandas, numpy
- scikit-learn
- matplotlib, seaborn

## 🔍 Visualization
- Boxplots
- Actual vs Predicted scatter plot with regression line
