
# Stroke Risk Prediction Using Machine Learning

## Project Overview
This project builds a machine learning model to predict stroke risk using patient demographic and health information.

## Dataset
Stroke prediction dataset containing 5,109 patient records.

Features include:
- Age
- Hypertension
- Heart Disease
- BMI
- Average Glucose Level
- Smoking Status
- Work Type
- Residence Type

## Techniques Used
- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Encoding
- Handling Class Imbalance using SMOTE
- Machine Learning Models:
  - Logistic Regression
  - Random Forest
  - XGBoost
  - KNN
  - Decision Tree

## Model Evaluation
- Confusion Matrix
- ROC Curve

## Tools
Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
## Model Results (After Hyperparameter Tuning)

| Model | Accuracy | ROC-AUC |
|---|---|---|
| Random Forest | 90% | 0.56 |
| XGBoost | 89% | 0.56 |
| Decision Tree | 86% | 0.53 |
| KNN | 79% | 0.56 |
| Logistic Regression | 77% | 0.74 |

**Best overall:** Random Forest (highest accuracy)
**Best for detecting stroke cases:** Logistic Regression (highest ROC-AUC — critical for imbalanced medical data)

Handled severe class imbalance (95:5 ratio) using SMOTE on 5,109 patient records.
