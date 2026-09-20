# ❤️ Heart Disease Prediction using Logistic Regression

## 🩺 Project Overview

This project aims to develop a **Logistic Regression** based Machine Learning model to **predict the 10-year risk of Coronary Heart Disease (CHD)** in patients using their medical and lifestyle attributes.

By leveraging the **Framingham Heart Study dataset**, this model serves as a simple and interpretable tool to assist in early detection and prevention of heart disease.


## 📊 Dataset: Framingham Heart Study

- The dataset includes anonymized health information from patients including:
  - Age, gender, smoking habits, cholesterol levels, blood pressure, BMI, glucose, etc.
- Target column: `TenYearCHD` (0 = No heart disease, 1 = Likely heart disease in 10 years)


## 🎯 Project Goals

### ✅ 1. Import Libraries & Dataset
- Load libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`
- Load dataset and explore structure
- Drop unnecessary column (`education`)
- Rename columns for readability

### ✅ 2. Data Preprocessing
- Drop missing values
- Scale numerical features using `StandardScaler`
- Split dataset into **train (70%)** and **test (30%)** sets

### ✅ 3. Exploratory Data Analysis (EDA)
- Class distribution of CHD
- Correlation heatmap
- Identify important risk factors (e.g., age, cholesterol, blood pressure, smoking, glucose)

### ✅ 4. Model Training
- Train a **Logistic Regression** model using scikit-learn
- Use `Binary Cross-Entropy Loss` (built-in for logistic regression)

### ✅ 5. Model Evaluation
- Evaluation metrics:
  - Accuracy
  - Precision
  - Recall
  - F1-Score
  - Confusion Matrix
  - ROC-AUC Score
- Visualize ROC Curve
- Predict heart disease risk for new patient data


## 📈 Results

- **Model Performance:**
  - Accuracy ~ 84%
  - ROC-AUC Score ~ 0.79
- The model successfully identifies key risk indicators and can be used as a baseline for CHD prediction.


## 💡 Future Improvements

- Use **Ensemble Methods** like:
  - Random Forest
  - XGBoost
  - Gradient Boosting
- Handle class imbalance using:
  - SMOTE (Synthetic Minority Over-sampling)
  - Class weight adjustments

## 🗂️ Project Structure

Heart_Disease_Prediction/
├── data/
│ └── framingham.csv
├── notebook/
│ └── heart_disease_logistic_regression.ipynb
├── models/
│ └── logistic_model.pkl
├── README.md
└── requirements.txt
