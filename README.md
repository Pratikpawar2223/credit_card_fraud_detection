Credit Card Fraud Detection
Table of Contents

Dataset

Feature Description

Target Variable

Results

Conclusion

Dataset

This dataset contains credit card transactions and is used to identify fraudulent transactions.

Total features: 22

Target variable: is_fraud

The dataset includes customer information, transaction details, and merchant details.

Feature Description
Feature	Description
trans_date_trans_time	Transaction date and time
cc_num	Credit card number
merchant	Merchant name
category	Merchant category type
amt	Transaction amount
first	Customer first name
last	Customer last name
gender	Customer gender
street	Customer street address
city	Customer city
state	Customer state
zip	Customer postal code
lat	Customer latitude
long	Customer longitude
city_pop	Population of the customer’s city
job	Customer job
dob	Customer date of birth
trans_num	Transaction number
unix_time	Transaction time in Unix format
merch_lat	Merchant latitude
merch_long	Merchant longitude
age	Customer age
Target Variable
Variable	Description
is_fraud	Indicates whether a transaction is fraudulent
1	Fraudulent transaction
0	Non-fraudulent transaction
Results
Model	Accuracy	ROC AUC	Precision	Recall	F1 Score	Notes
Logistic Regression	0.92	-	-	-	-	Baseline linear model
Random Forest Classifier	0.99	-	-	-	-	Strong performance
XGBoost	0.9994	0.9808	0.9583	0.7041	0.8118	Best model selected
SVM	Not evaluated	-	-	-	-	High computation time

Best threshold (F1 optimized) for XGBoost: 0.9077
Flagged transactions count: 72
Flagged transactions saved to: flagged_transactions.csv

Conclusion

XGBoost was the best performing model, achieving high precision (95.8%) and strong ROC-AUC (0.9808).

The threshold of 0.9077 balances false positives and detection rate, resulting in an F1 score of 0.8118.

The pipeline successfully flagged 72 potential fraudulent transactions for review.

Future improvements include:

Feature engineering

Hyperparameter tuning

Deployment for real-time credit card fraud detection
