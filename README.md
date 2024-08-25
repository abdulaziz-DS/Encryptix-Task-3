# Encryptix Task 3: Credit Card Fraud Detection

## Overview

This project aims to build a machine learning model to identify fraudulent credit card transactions. By analyzing transaction data, the goal is to develop a predictive model that accurately classifies transactions as fraudulent or genuine, enhancing security measures for financial systems.

## Dataset

The dataset used in this project consists of credit card transaction records with features such as transaction amount, time, and anonymized features. The dataset was provided in CSV format, and various preprocessing steps were applied to prepare it for modeling.

## Project Structure

### Data Preprocessing

- **Handling Missing Values**: The dataset was cleaned to address any missing values.
- **Normalization**: Features were normalized using StandardScaler to ensure consistent scale across all features.
- **Class Imbalance**: Applied SMOTE (Synthetic Minority Over-sampling Technique) to balance the classes.

### Feature Engineering

- The features were used directly in the model after preprocessing. Given their relevance to fraud detection, no additional feature engineering was performed.

### Modeling

- **Model Choice**: A Logistic Regression model was built to classify transactions as fraudulent or genuine.
- **Training and Testing**: The model was trained on a balanced dataset and evaluated on a test set.

### Evaluation

- **Metrics**: The model's performance was assessed using precision, recall, F1-score, and overall accuracy.

## Model and Results

The Logistic Regression model was trained and evaluated on the preprocessed data. The performance metrics are as follows:

### Without Undersampling

- **Precision**: 0.93 (genuine), 0.97 (fraudulent)
- **Recall**: 0.98 (genuine), 0.92 (fraudulent)
- **F1-Score**: 0.95 (genuine), 0.95 (fraudulent)
- **Accuracy**: 95%

### With Undersampling

- **Precision**: 0.91 (genuine), 0.96 (fraudulent)
- **Recall**: 0.96 (genuine), 0.90 (fraudulent)
- **F1-Score**: 0.94 (genuine), 0.93 (fraudulent)
- **Accuracy**: 93%

## Insights

The model demonstrates strong performance in detecting fraudulent transactions, with high precision and recall values. The balanced accuracy achieved through undersampling further improves the model’s reliability. There is potential for enhancing the model by exploring more sophisticated techniques or incorporating additional features.
