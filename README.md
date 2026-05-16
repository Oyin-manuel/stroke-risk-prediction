
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

Best Results after Hyperparameter Tuning:
Random Forest: 90% accuracy
Logistic Regression: Best ROC-AUC score (0.74)
Trained and compared 5 models: Logistic Regression, Decision Tree, Random Forest, KNN, XGBoost
Handled severe class imbalance (95:5 ratio) using SMOTE oversampling on 5,109 patient records
