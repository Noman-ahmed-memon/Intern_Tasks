# 🫀 Heart Disease Prediction

## 📌 Objective
Predict whether a person is at risk of heart disease based on health features such as age, cholesterol, blood pressure, chest pain type, and more.

## 📁 Dataset
- Source: UCI Heart Disease Dataset
- Format: CSV (`heart.csv`)
- Target Column: `HeartDisease` (1 = has disease, 0 = no disease)

## 📊 Features Used
- Age
- Sex
- Chest Pain Type
- Resting Blood Pressure
- Cholesterol
- Fasting Blood Sugar
- Resting ECG
- Max Heart Rate
- Exercise-Induced Angina
- Oldpeak
- ST Slope

## 🔍 Steps Performed
1. Data Cleaning (checked for missing values)
2. Exploratory Data Analysis (EDA)
3. Feature Encoding (used `pd.get_dummies`)
4. Train-test Split (80/20)
5. Model Training:
   - Logistic Regression
6. Model Evaluation:
   - Accuracy Score
   - Confusion Matrix
   - ROC Curve
   - Classification Report
7. Feature Importance Analysis

## 📈 Results
- Accuracy: 0.8532608695652174
- ROC-AUC: 0.92
- Most important features: *e.g., Age, Chest Pain Type, Oldpeak*

## 💻 Tools Used
- Python
- Pandas, Seaborn, Matplotlib
- Scikit-learn

