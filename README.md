# **CREDIT CARD FRAUD DETECTION 💳⚡**


Detect fraudulent credit card transactions using machine learning. This project leverages XGBoost for high-performance classification and flags suspicious transactions for further review.

## 📝 PROJECT OVERVIEW

This project aims to identify potential fraudulent transactions in credit card datasets. Using machine learning, it helps minimize financial loss and ensures transaction security.
## 📊 RESULTS
| Metric                   | Value   |
| ------------------------ | ------- |
| **Best Model**           | XGBoost |
| **Best Threshold (F1)**  | 0.9077  |
| **Accuracy**             | 0.9994  |
| **ROC AUC**              | 0.9808  |
| **Precision**            | 0.9583  |
| **Recall**               | 0.7041  |
| **F1 Score**             | 0.8118  |
| **Flagged Transactions** | 72      |
The model achieves high precision and a balanced F1 score, making it reliable for detecting fraudulent transactions.

## 📂 FILES

flagged_transactions.csv – Contains all transactions flagged as potentially fraudulent.

credit_card_fraud_detection.py – Python script with full code and analysis (designed for VS Code).

## ▶️ HOW TO RUN

Clone the repository:

git clone <your-repo-url>


Open credit_card_fraud_detection.py in VS Code.

Run the script to detect fraudulent transactions and save them to flagged_transactions.csv.

## ✅ CONCLUSION

The XGBoost model successfully identifies suspicious transactions with high accuracy and precision. While recall is slightly lower, the high F1 score ensures a good balance between catching frauds and minimizing false alarms. This system can be used as a real-time fraud detection tool to protect credit card users.


## 🛠 TECHNOLOGIES USED
Python 3.x

XGBoost

Pandas & NumPy

Scikit-learn

VS Code
