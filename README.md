Credit Card Fraud Detection using Machine Learning
Project Overview

This project focuses on detecting fraudulent credit card transactions using machine learning techniques.

The dataset contains anonymized transaction data with a highly imbalanced class distribution, where fraudulent transactions are very rare compared to legitimate ones. The goal is to build a model that can accurately identify fraud while minimizing false positives.

The final model allows prediction of:

• Whether a transaction is fraudulent or not
• Probability of fraud
• Key features influencing the prediction

This project demonstrates the application of artificial intelligence in financial fraud detection systems.

Research Workflow

The project follows a structured machine learning pipeline.

1. Data Collection

The dataset used is a publicly available Credit Card Fraud Dataset from Kaggle.

Contains transaction data from real credit card transactions
Features are anonymized using PCA transformation
Includes both fraudulent and non-fraudulent transactions
2. Data Understanding

Initial exploration was performed to understand the dataset structure:

Total number of transactions
Number of fraud vs non-fraud cases
Feature distribution analysis
Detection of missing values and anomalies
3. Data Preprocessing

Data preprocessing is a critical step due to class imbalance and feature scaling requirements.

Handling missing values
Feature scaling (StandardScaler / normalization)
Handling imbalanced data using:
SMOTE (Synthetic Minority Oversampling Technique)
Undersampling
Combination methods
4. Exploratory Data Analysis (EDA)

EDA was performed to understand patterns in the data:

Distribution of fraud vs non-fraud transactions
Correlation analysis between features
Visualization of transaction patterns
Detection of important features
5. Model Training

Machine learning models were trained to detect fraud:

Logistic Regression
Random Forest

Models were trained on:

Original imbalanced data
Balanced data (SMOTE)
Undersampled data
6. Model Evaluation

Models were evaluated using appropriate metrics for imbalanced data:

Accuracy
Precision
Recall
F1-score
ROC-AUC

Special focus was given to Recall and Precision, as detecting fraud correctly is more important than overall accuracy.

AI Prediction Model

The final system predicts fraud in real-time based on transaction data.

Input Variables
Transaction features (V1, V2, ..., V28)
Transaction amount
Scaled features
Output

The model provides:

• Fraud probability score
• Prediction (Fraud / Not Fraud)
• Feature importance (for interpretability)

Project Structure

Credit_Card_Fraud_Detection
│
├── data
│ ├── raw_dataset.csv
│ └── processed_dataset.csv
│
├── notebooks
│ ├── EDA.ipynb
│ ├── Preprocessing.ipynb
│ └── ModelTraining.ipynb
│
├── models
│ ├── logistic_regression.pkl
│ └── random_forest.pkl
│
├── figures
│ ├── eda_plots.png
│ └── feature_importance.png
│
├── app
│ └── app.py
