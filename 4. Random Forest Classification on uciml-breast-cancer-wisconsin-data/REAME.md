### Random Forest Classification on uciml/breast-cancer-wisconsin-data

This project documents the development of a machine learning workflow for classifying breast cancer tumors using the UCI Breast Cancer Wisconsin dataset.

#### Key Information & Decisions
* **Dataset:** The `uciml/breast-cancer-wisconsin-data` was used.
* **Preprocessing:** 
    * Irrelevant columns were removed.
    * Diagnosis codes 'B' and 'M' were replaced with "benign" and "malignant".
    * Features were normalized using `StandardScaler`.
* **Modeling:** A `RandomForestClassifier` was trained, achieving an **accuracy of 96.49%**.
* **Evaluation:**
<img width="640" height="547" alt="image" src="https://github.com/user-attachments/assets/4d3a5aab-55d7-47ac-9b97-ce58f7274d2a" />

