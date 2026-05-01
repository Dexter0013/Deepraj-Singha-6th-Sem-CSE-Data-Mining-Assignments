# SMS Spam Detection Project

## Overview
This project implements a machine learning model to classify SMS messages as either **Spam** or **Not Spam (Ham)**. It uses the SMS Spam Collection dataset and utilizes Natural Language Processing (NLP) techniques to process text and a Naive Bayes classifier for prediction.

## Dataset
- **Source:** [UCI SMS Spam Collection Dataset](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)
- **Format:** CSV with label and message columns.
- **Size:** 5,572 messages.

## Methodology
1. **Data Preprocessing:**
   - Cleaned the dataset by removing unnecessary columns.
   - Encoded labels: `Spam` (1) and `Not Spam` (0).
   - Split the data into training (80%) and testing (20%) sets using stratified sampling.
2. **Feature Extraction:**
   - Used `TfidfVectorizer` to convert text into numerical features.
   - Applied English stop-word removal and lowercase normalization.
3. **Model Training:**
   - Implemented a `MultinomialNB` (Naive Bayes) classifier, which is highly efficient for text-based categorical data.

## Results
- **Accuracy:** ~96.86%
- **Precision for Spam:** 1.00 (Zero false positives in testing).
- **Recall for Spam:** 0.77 (Caught 77% of all spam messages).

### Confusion Matrix
<img width="510" height="393" alt="image" src="https://github.com/user-attachments/assets/1bd190d0-a14e-4bf6-9e5a-724e0fd99b18" />

- **True Negatives:** 966 (Legitimate messages correctly identified)
- **True Positives:** 114 (Spam messages correctly identified)
- **False Positives:** 0 (Legitimate messages mistakenly blocked)
- **False Negatives:** 35 (Spam messages that slipped through)
