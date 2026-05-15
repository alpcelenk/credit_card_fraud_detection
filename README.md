# Credit Card Fraud Detection

This project focuses on detecting fraudulent credit card transactions using machine learning classification models.

The goal of the project is to identify whether a transaction is fraudulent (`1`) or legitimate (`0`) based on transaction-related features.

---

# Dataset

The dataset contains real credit card transactions made by European cardholders in September 2013.

- Total Transactions: 284,807
- Fraudulent Transactions: 492
- Fraud Ratio: 0.172%

The dataset is highly imbalanced, making fraud detection a challenging classification problem.

Dataset Link:

[Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

---

# Project Workflow

## 1. Data Preprocessing

The following preprocessing steps were applied:

- Missing value check
- Removing unnecessary features (`Time`)
- Feature scaling for `Amount`
- Train-test split with stratified sampling

---

# Models Used

The following classification models were tested during the project:

- Logistic Regression
- Random Forest Classifier

Among these models, **Random Forest Classifier** achieved the best overall fraud detection performance.

---

# Model Performance

## Logistic Regression

| Metric | Score |
|---|---|
| Precision | 0.84 |
| Recall | 0.66 |
| F1-Score | 0.74 |

---

## Random Forest Classifier

| Metric | Score |
|---|---|
| Precision | 0.97 |
| Recall | 0.72 |
| F1-Score | 0.83 |
| ROC-AUC | 0.949 |

---

# Key Insight

Since the dataset is highly imbalanced, accuracy alone is not a reliable evaluation metric.

Instead, the project focuses on:
- Precision
- Recall
- F1-Score
- ROC-AUC

Especially in fraud detection systems, recall is important because missing fraudulent transactions can lead to significant financial loss.

---

# Visualizations

The project includes several visualizations such as:

- Fraud distribution analysis
- Confusion matrix

---

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

# Conclusion

The Random Forest model achieved strong fraud detection performance with a ROC-AUC score of approximately **0.95**.
