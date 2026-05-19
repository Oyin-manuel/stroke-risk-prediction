# Stroke Risk Prediction Using Machine Learning

## 📌 Project Overview
Stroke is one of the leading causes of death and disability globally. Early prediction of high-risk factors can significantly improve patient outcomes and save lives. 

This project develops an end-to-end machine learning pipeline to predict a patient's stroke risk using demographic, lifestyle, and clinical health data. 

## 📊 Dataset & Feature Breakdown
The project utilizes a clinical dataset containing **5,109 patient records** with 11 distinct attributes:
* **Demographics:** Age, Gender, Work Type, Residence Type, Marital Status
* **Clinical Indicators:** Hypertension, Heart Disease, BMI, Average Glucose Level
* **Lifestyle Factors:** Smoking Status

## 🛠️ Data Challenges & Advanced Techniques Used
Real-world medical data is inherently messy and highly skewed. This project directly handles those complexities using:
* **Handling Class Imbalance:** The dataset suffers from a severe **95:5 class imbalance** (only 5% of records represent stroke cases). To prevent model bias, **SMOTE (Synthetic Minority Over-sampling Technique)** was applied to balance the training data.
* **Data Cleaning & Preprocessing:** Handled missing clinical values (such as `bmi` inputs) and utilized robust scaling for continuous variables like glucose levels.
* **Feature Engineering & Encoding:** Transformed categorical string variables into analytical numerical markers using Target/One-Hot encoding.
* **Exploratory Data Analysis (EDA):** Leveraged `Matplotlib` and `Seaborn` to isolate key correlations—notably tracking how advanced age and high average glucose levels heavily compound stroke risks.

## 🤖 Machine Learning Frameworks & Models Evaluated
Five distinct classification algorithms were implemented, tuned, and evaluated:
1.  Logistic Regression
2.  Random Forest Classifier
3.  XGBoost Classifier
4.  K-Nearest Neighbors (KNN)
5.  Decision Trees

## 📈 Model Performance & Evaluation Metrics
After rigorous hyperparameter tuning, the models yielded the following results:

| Model | Accuracy | ROC-AUC |
| :--- | :---: | :---: |
| **Random Forest** | **90%** | 0.56 |
| **XGBoost** | 89% | 0.56 |
| **Decision Tree** | 86% | 0.53 |
| **KNN** | 79% | 0.56 |
| **Logistic Regression** | 77% | **0.74** |

### 🔍 Key Technical Takeaway:
While tree-based models like **Random Forest** yielded the highest overall structural *Accuracy (90%)*, they struggled with sensitivity due to the skewed nature of the data. 

For clinical applications, **Logistic Regression** emerged as the most viable baseline model due to its significantly higher **ROC-AUC of 0.74**. In a healthcare context, maximizing the area under the ROC curve is critical because it minimizes false negatives, ensuring fewer high-risk stroke patients are missed by the system.

## 🧰 Tech Stack Used
* **Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-Learn, XGBoost, Imbalanced-Learn (SMOTE)
* **Visualization:** Matplotlib, Seaborn
* **Environment:** Jupyter Notebook
* 
