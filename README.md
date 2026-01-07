
# Heart Disease Prediction using Machine Learning

## Author
**Devadevan S**

## Project Overview
Heart disease is one of the leading causes of death worldwide. Early detection can significantly reduce risks and improve patient outcomes.  
This project implements a Machine Learning–based Heart Disease Prediction system using clinical and medical attributes to predict whether a patient is likely to have heart disease.

The project demonstrates a complete end-to-end ML pipeline including data preprocessing, model training, evaluation, interpretation, and deployment readiness.

---

## Problem Statement
To develop a supervised machine learning model that predicts the presence or absence of heart disease based on patient medical data.

**Type:** Binary Classification  
**Target Variable:** Heart Disease (0 = No, 1 = Yes)

---

## Dataset
- File: `Heart_Disease_Prediction.csv`
- Each row represents a patient
- Each column represents a medical attribute such as age, cholesterol, blood pressure, heart rate, etc.

---

## Technologies Used
- Python
- Google Colaboratory
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Joblib
- FastAPI (for deployment readiness)

---

## Data Preprocessing
- Checked for missing values and handled them appropriately
- Encoded categorical variables into numerical form
- Applied feature scaling using StandardScaler
- Split data into training and testing sets

---

## Models Implemented
- Logistic Regression
- Decision Tree
- Random Forest (Final Model)

### Why Random Forest?
- Handles non-linear relationships effectively
- Reduces overfitting through ensemble learning
- Provides feature importance for interpretability
- Achieved better F1-score compared to other models

---

## Model Evaluation
The model was evaluated using:
- Accuracy
- Precision
- Recall
- F1-score

F1-score was emphasized because it balances false positives and false negatives, which is critical in healthcare-related predictions.

---

## Feature Importance
Feature importance analysis showed that attributes such as chest pain type, maximum heart rate, cholesterol level, and age significantly impact heart disease prediction.

---

## Deployment / API (Conceptual)
The trained model can be deployed using Flask or FastAPI:
- Input: Patient medical details
- Output: Heart disease prediction in JSON format

The trained model is saved using Joblib for reuse in production.

---
