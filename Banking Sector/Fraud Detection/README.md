# Fraud Detection Project

## Overview
This project is a **machine learning pipeline** designed to detect fraudulent transactions in financial datasets. The solution leverages various algorithms and techniques to maximize accuracy and performance. The pipeline includes data preprocessing, training, evaluation, and comparison of models under two scenarios:
1. **Filtered Transactions**: Focuses on specific transaction patterns where fraud is more likely.
2. **Unfiltered Transactions**: Includes all transaction types for broader analysis.

## Objective
The main goal is to develop a robust system to identify fraudulent activities while minimizing false positives. This is achieved by experimenting with multiple machine learning algorithms and comparing their performance under the two scenarios mentioned above.

---

## Algorithms Used
1. **Logistic Regression**
2. **Random Forest Classifier**
3. **Support Vector Classifier (SVC)**
4. **XGBoost Classifier**

These algorithms were chosen for their diverse strengths in handling imbalanced datasets and their interpretability in the context of fraud detection.

---

## Methodology
### 1. Data Preprocessing
- **Initial Filtering**: Fraud was observed to occur only in `Transfer` and `Cash Out` transactions. The filtered version of the dataset focuses on these two transaction types.
- **Handling Imbalance**: Synthetic Minority Over-sampling Technique (**SMOTE**) was applied to balance the dataset for training.

### 2. Model Training and Evaluation
- **Training**: Models were trained using the filtered and unfiltered datasets.
- **Evaluation Metrics**:
  - Accuracy
  - Precision
  - Recall
  - F1 Score
  - Area Under the Receiver Operating Characteristic (ROC-AUC)

### 3. Comparison
The performance of the models was analyzed and compared across the two scenarios (filtered vs. unfiltered datasets) to understand the impact of filtering transaction patterns on fraud detection.

---

## Results
- The results highlight how the inclusion or exclusion of specific transaction types affects model performance.
- Insights on the strengths and weaknesses of each algorithm were documented.
