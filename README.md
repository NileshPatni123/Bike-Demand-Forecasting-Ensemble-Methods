# Bike-Demand-Forecasting-Ensemble-Methods
Comparison of Bagging, Subagging, and Boosting ensemble regression models for hourly bike demand forecasting using K-Fold cross validation.

## Student Name:
Nilesh Patni

---

## 📌 Objective

The objective of this assignment is to predict hourly bike rental demand using ensemble regression methods and compare their performance using K-Fold Cross Validation.

---

## 📊 Dataset

Dataset: UCI Bike Sharing Dataset  
File Used: hour.csv  
Target Variable: cnt (hourly bike rental count)

---

## 🧠 Models Implemented

1. Bagging:
   - RandomForestRegressor

2. Subagging:
   - BaggingRegressor (max_samples < 1.0)

3. Boosting:
   - GradientBoostingRegressor

---

## 🔁 Evaluation Method

- K-Fold Cross Validation (k = 5)
- Metrics Used:
  - RMSE (Root Mean Squared Error)
  - MAE (Mean Absolute Error)

---

## ⚙ Hyperparameters Tuned

### Random Forest
- n_estimators
- max_depth

### Subagging
- n_estimators
- max_samples

### Boosting
- n_estimators
- learning_rate

---

## 📈 Output Files

- cv_regression_results.csv  
  → Contains mean ± std of RMSE and MAE for each model

- final_predictions.csv  
  → Contains:
    - ActualCnt
    - PredictedCnt

---

## 🔍 Feature Importance

Top 8 important features were extracted using tree-based importance scores.

---

## 📌 Conclusion Summary

Boosting typically generalizes better because:
- It reduces bias by sequentially correcting previous errors.
- It balances bias–variance tradeoff effectively.

Random Forest reduces variance through averaging.
Subagging improves stability but may have slightly higher bias.

---

## 📂 Files Included

- task3_bike_regression_ensembles.py
- hour.csv
- cv_regression_results.csv
- final_predictions.csv
- README.md
- Report.pdf
