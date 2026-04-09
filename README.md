# Credit Card Fraud Detection using Machine Learning

## Project Overview

This project focuses on detecting **fraudulent credit card transactions** using Machine Learning techniques.

The dataset contains anonymized transaction data with a **highly imbalanced class distribution**, where fraudulent transactions are significantly rarer than legitimate ones.

### Objective:
Build a robust model that:
- Accurately identifies fraudulent transactions  
- Minimizes false positives  
- Works effectively on imbalanced data  

---

## Key Capabilities

- ✔ Predict whether a transaction is **Fraudulent or Legitimate**  
- ✔ Provide **fraud probability score**  
- ✔ Identify **important features influencing predictions**  

This project demonstrates the **real-world application of AI in financial fraud detection systems**.

---

## Machine Learning Workflow

### 1️⃣ Data Collection
- Dataset sourced from **Kaggle Credit Card Fraud Dataset**  
- Contains real-world transaction data  
- Features anonymized using **PCA transformation**  
- Includes both fraudulent and non-fraudulent transactions  

---

### 2️⃣ Data Understanding

Initial exploration included:
- Total number of transactions  
- Fraud vs non-fraud distribution  
- Feature distribution analysis  
- Detection of missing values and anomalies  

---

### 3️⃣ Data Preprocessing

Due to class imbalance, preprocessing is critical:

- Handling missing values  
- Feature scaling (StandardScaler / Normalization)  

#### Handling imbalanced data using:
- SMOTE (Synthetic Minority Oversampling Technique)  
- Undersampling  
- Hybrid approaches  

---

### 4️⃣ Exploratory Data Analysis (EDA)

EDA was conducted to uncover patterns:

- Fraud vs non-fraud distribution  
- Correlation between features  
- Visualization of transaction behaviors  
- Identification of important features  

---

### 5️⃣ Model Training

The following models were trained:

- Logistic Regression  
- Random Forest  

#### Training performed on:
- Original imbalanced dataset  
- SMOTE-balanced dataset  
- Undersampled dataset  

---

### 6️⃣ Model Evaluation

Evaluation metrics suitable for imbalanced datasets:

- Accuracy  
- Precision  
- Recall  
- F1-Score  
- ROC-AUC  

**Important:**  
Special emphasis was placed on **Recall and Precision**, since detecting fraud is more critical than overall accuracy.

---

## AI Prediction System

The final model enables **real-time fraud detection**.

---

### Input Features
- Transaction features: `V1, V2, ..., V28`  
- Transaction Amount  
- Scaled/processed features  

---

### Output
- Fraud Probability Score  
- Prediction: **Fraud / Not Fraud**  
- Feature Importance (for interpretability)  

---

## Tech Stack
- Python 
- Scikit-learn  
- Pandas & NumPy  
- Matplotlib & Seaborn  

---

## Use Cases

- Banking fraud detection systems  
- Payment gateway security  
- Real-time transaction monitoring  

---

## Conclusion

This project highlights how Machine Learning can be effectively used to:
- Detect rare fraudulent events  
- Handle highly imbalanced datasets  
- Build reliable and interpretable fraud detection systems  

---
