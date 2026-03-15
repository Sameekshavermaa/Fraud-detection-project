# Credit Card Fraud Detection

This project builds a machine learning model to detect fraudulent credit card transactions.

## Model Used
Random Forest Classifier

## Dataset
European cardholder transaction dataset.

## Features
- Data preprocessing
- Fraud detection model
- Precision and recall evaluation
- Confusion matrix visualization

## Goal
Build a real-world AI fraud detection system.
## Dataset Explanation

The dataset used in this project contains credit card transactions made by European cardholders.

It includes both normal and fraudulent transactions collected over two days.

### Dataset Characteristics

- Total Transactions: 284,807
- Fraudulent Transactions: 492
- Fraud Percentage: 0.172%

This dataset is highly **imbalanced**, meaning fraudulent transactions are extremely rare compared to normal ones.

### Features

The dataset contains **30 features**:

- `Time` – seconds elapsed between transactions
- `Amount` – transaction amount
- `V1` to `V28` – anonymized features created using PCA transformation
- `Class` – target variable  
  - `0` → Normal Transaction  
  - `1` → Fraudulent Transaction

### Challenge

Because fraud cases are rare, the machine learning model must handle **class imbalance** effectively to detect fraud accurately.
## Model Results

After preprocessing the dataset, a **Random Forest Classifier** was trained to identify fraudulent transactions.

### Model Performance

- Accuracy: 99.96%
- Precision (Fraud Detection): 92%
- Recall (Fraud Detection): 85%
- F1 Score: 88%

### Interpretation

The model performs very well in identifying fraudulent transactions while maintaining a low number of false positives.

Since the dataset is highly imbalanced, evaluation metrics like **Precision**, **Recall**, and **F1-score** are more important than accuracy alone.

## Confusion Matrix

The confusion matrix shows the performance of the fraud detection model.

![Confusion Matrix]([images/confusion-matrix.png](https://github.com/Sameekshavermaa/Fraud-detection-project/blob/b4211bb57ca63b3212590accebc9b990bb7f6d63/images%3Aconfusion-matrix.png))
