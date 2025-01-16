# Fraud Detection Project

## Overview
This project is a **machine learning project** designed to detect fraudulent transactions in a financial dataset. The solution leverages various algorithms and techniques to maximize accuracy and performance. The project includes descriptive analysis, data preprocessing, training, evaluation, and comparison of models under two scenarios:
1. [**Filtered Transactions**](https://github.com/MPeredaPerea/Machine_learning_projects/blob/main/Banking%20Sector/Fraud%20Detection/Fraud_Detection_Filtering.ipynb): Focuses on specific transaction patterns where fraud is more likely.
2. [**Unfiltered Transactions**](https://github.com/MPeredaPerea/Machine_learning_projects/blob/main/Banking%20Sector/Fraud%20Detection/Fraud_Detection.ipynb): Includes all transaction types for broader analysis.

This project is a test, as the results are not entirely interpretable due to the low number of class 1 (fraud) samples.

## Objective
The main goal is to develop a robust system to identify fraudulent activities while minimizing false positives. This is achieved by experimenting with multiple machine learning algorithms and comparing their performance under the two scenarios mentioned above.

---

## Algorithms Used
1. **Logistic Regression**
2. **Decision Tree**
3. **Random Forest Classifier**
4. **XGBoost Classifier**
5. **Kneighbors Classifier**
6. **Support Vector Classifier (SVC)**

---

## Methodology
### 1. Descriptive Analysis
- Understand the information in the dataset.
- Find patterns to identify Fraud
### 2. Data Preprocessing
- **Initial Filtering** (For the Filtered Notebook): Fraud was observed to occur only in `Transfer` and `Cash Out` transactions. The filtered version of the dataset focuses on these two transaction types.
- **Handling Imbalance**: Synthetic Minority Over-sampling Technique (**SMOTE**) was applied to balance the dataset for training.

### 3. Model Training and Evaluation
- **Training**: Models were trained using the filtered and unfiltered datasets.
- **Evaluation Metrics**:
  - Accuracy
  - Precision
  - Recall
  - F1 Score
  - Area Under the Receiver Operating Characteristic (ROC-AUC)

### 4. Comparison
The performance of the models was analyzed and compared across the two scenarios (filtered vs. unfiltered datasets) to understand the impact of filtering transaction patterns on fraud detection.

---

## Results

- As said before, there are not enough Class 1 (Fraud) values in the test sample to make conclussions. So, this is a test to show how results should have been interpretated for a dataset with more Fraud values.

- Results Interpretation: The most important metric is the class 1 Recall value, it shows how many Frauds have been predicted as no Fraud.

- The results highlight how the inclusion or exclusion of specific transaction types affects model performance.

- Non Filtered Results
![Non Filtered Results](https://github.com/MPeredaPerea/Machine_learning_projects/blob/main/Banking%20Sector/Fraud%20Detection/Images/normal.png)

- Filtered Results
![Filtered Results](https://github.com/MPeredaPerea/Machine_learning_projects/blob/main/Banking%20Sector/Fraud%20Detection/Images/filtered.png)

- In my opinion, the best result obtained is using the Logistic Regression Algorithm for the non Filtered Dataset. It is true that it makes so many wrong predictions, but at least is the one with the highest amount of true Fraud detections. The objective should be to mantain or increase this Recall value, while improving the Accuracy Metric.
![Logistic Regression ALG](https://github.com/user-attachments/assets/d4f3fcb2-f950-480a-b69e-7df992e45a19)

  

