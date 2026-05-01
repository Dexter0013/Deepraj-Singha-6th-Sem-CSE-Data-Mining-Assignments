# Iris Species Classification using KNN

This repository contains a machine learning project that classifies Iris flower species using the K-Nearest Neighbors (KNN) algorithm.

## Project Overview
The goal of this project was to build a robust classification model for the classic Iris dataset. The workflow involved data preprocessing, feature scaling, hyperparameter tuning, and visual evaluation.

## Key Features
- **Algorithm:** K-Nearest Neighbors (KNN)
- **Preprocessing:** Feature scaling using `StandardScaler` to ensure distance metrics are unbiased.
- **Optimization:** Hyperparameter tuning to find the optimal $k$ value ($k=17$).
- **Evaluation:** Comprehensive reporting including Accuracy, F1-Score, and a Confusion Matrix.

## Results
The final model achieved an accuracy of **96.67%** on the test set.

### Classification Report
```
              precision    recall  f1-score   support

      setosa       1.00      1.00      1.00        10
  versicolor       1.00      0.90      0.95        10
   virginica       0.91      1.00      0.95        10
```

## Visualizations
<img width="640" height="547" alt="image" src="https://github.com/user-attachments/assets/4b9ad53f-9d27-4f04-8c1e-12426493dd11" />
