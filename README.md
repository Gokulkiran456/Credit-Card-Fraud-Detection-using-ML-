# Credit-Card-Fraud-Detection-using-ML-
Overview
Credit card fraud is a significant challenge faced by financial institutions worldwide. This project leverages machine learning techniques to classify fraudulent and non-fraudulent transactions using the Kaggle Credit Card Fraud Dataset. The goal is to build a robust classifier capable of detecting fraudulent transactions in imbalanced datasets.

Dataset
The dataset contains transactions made by European cardholders in September 2013.
It is highly imbalanced, with 0.17% of transactions classified as fraud.
Features include 28 anonymized principal components obtained via PCA (V1 to V28), Time, and Amount.
The target variable is Class:
0: Non-Fraudulent
1: Fraudulent
Source: Kaggle Credit Card Fraud Detection Dataset

Project Workflow
Exploratory Data Analysis (EDA):

Examined class distribution and feature correlations.
Identified the need for class balancing due to extreme imbalance.
Data Preprocessing:

Standardized numerical features using StandardScaler.
Handled class imbalance using SMOTE (Synthetic Minority Oversampling Technique).
Model Training:

Built and trained a Random Forest Classifier on the resampled dataset.
Evaluated model performance using metrics like Precision, Recall, F1-Score, and ROC-AUC.
Evaluation:

Used a confusion matrix and classification report for performance analysis.
Plotted feature importances to understand the contribution of each variable.
Model Deployment:

Saved the trained model and scaler using joblib for deployment.
Key Results
Model Performance:

Precision: ~99% for Non-Fraudulent, ~85% for Fraudulent.
Recall: ~98% for Non-Fraudulent, ~91% for Fraudulent.
ROC-AUC Score: ~0.98.
Feature Importance:

Key features identified include V12, V14, and Amount.
