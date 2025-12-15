# 🩺 Diabetes Prediction Challenge

## 📌 Project Overview
Diabetes is a chronic disease that can lead to serious health complications if not detected early. With the help of machine learning and patient health data, this project aims to predict whether an individual is likely to be diagnosed with diabetes. The model uses demographic, lifestyle, and medical features to support early risk identification and preventive healthcare decisions.

---

## 🎯 Business Problem
Traditional diabetes diagnosis often happens after symptoms appear, which may be too late to prevent complications. Healthcare systems need a data-driven approach to:

- Identify high-risk individuals early
- Support preventive healthcare decisions
- Reduce long-term treatment costs
- Improve patient lifestyle awareness

---

## ✅ Project Objective
The objectives of this project are:
- To analyze large-scale patient health data
- To identify key factors influencing diabetes
- To perform Exploratory Data Analysis (EDA)
- To build and compare machine learning models
- To predict diabetes outcomes for unseen data
- To generate insights that support healthcare decision-making

---

## 📊 Dataset Description
The dataset contains patient-level health and lifestyle information and is divided into three files:

| Dataset | Rows | Columns | Description |
|------|------|--------|------------|
| Train | 700,000 | 26 | Used for model training and validation |
| Test | 300,000 | 25 | Used for prediction |
| Sample Submission | 300,000 | 2 | Defines submission format |

### 🔹 Target Variable
- **diagnosed_diabetes**
  - `0` → Not Diabetic
  - `1` → Diabetic

---

## 🧾 Feature Categories

### 👤 Demographic Features
- Age  
- Gender  
- Ethnicity  
- Education Level  
- Income Level  
- Employment Status  

### 🧘 Lifestyle Features
- Alcohol Consumption per Week  
- Physical Activity Minutes per Week  
- Diet Score  
- Sleep Hours per Day  
- Screen Time per Day  
- Smoking Status  

### ❤️ Medical & Clinical Features
- BMI  
- Waist-to-Hip Ratio  
- Systolic Blood Pressure  
- Diastolic Blood Pressure  
- Heart Rate  
- Cholesterol (Total, HDL, LDL)  
- Triglycerides  

### 🏥 Medical History
- Family History of Diabetes  
- Hypertension History  
- Cardiovascular History  

---

## 🔍 Exploratory Data Analysis (EDA)

EDA was performed to understand data patterns and relationships.

### 🔑 Key Insights from EDA
- Dataset is clean with **no missing values**
- Higher **BMI and waist-to-hip ratio** are strongly associated with diabetes
- **Age** is a major contributing factor
- Individuals with **family history of diabetes** show higher risk
- Poor **physical activity and diet score** increase diabetes probability
- High **blood pressure and cholesterol levels** are common among diabetic patients

EDA helped in identifying important features and understanding data behavior.

---

## 🛠 Data Preprocessing
The following preprocessing steps were applied:

- Dropped non-informative `id` column
- Scaled numerical features using **StandardScaler**
- Encoded categorical features using **One-Hot Encoding**
- Performed stratified train-validation split to maintain class balance

These steps ensured the data was model-ready and improved performance.

---

## 🤖 Machine Learning Models

### Models Implemented
1. **Logistic Regression**
   - Used as a baseline model
   - Simple and interpretable

2. **Random Forest Classifier**
   - Handles non-linear relationships
   - Works efficiently on large datasets
   - Delivered better performance than baseline

---

## 📈 Model Evaluation
Models were evaluated using:
- Accuracy
- ROC-AUC Score

Random Forest achieved higher ROC-AUC, making it the final selected model.

---

## 📤 Prediction & Submission
- Final model trained on the complete training dataset
- Predictions generated for test data
- Submission file created following Kaggle format

---

## 💡 Business & Healthcare Impact
This project demonstrates how machine learning can:
- Assist in early diabetes risk screening
- Support healthcare professionals with data-driven insights
- Encourage preventive lifestyle changes
- Reduce long-term healthcare costs

> ⚠️ This model is a **decision-support tool**, not a medical diagnosis system.

---

## 🧰 Tools & Technologies Used
- Python
- Pandas & NumPy
- Matplotlib & Seaborn
- Scikit-learn
- Kaggle Notebook Environment

---

## 🏁 Conclusion
This project presents an end-to-end data science workflow for healthcare prediction. By combining EDA, preprocessing, and machine learning models, a reliable diabetes prediction system was developed. The insights gained can help support preventive healthcare planning and early intervention.

---


