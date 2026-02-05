Credit Card Fraud Detection
Table of Contents:

Data Set

Code & Implementation

Result

Data Set
This dataset contains information about credit card transactions, including details of fraudulent activities. This dataset contains total 22 features:

Categorical Features:
trans_date_trans_time: shows the transaction time and date
cc_num: contains credit card number
merchant: merchant name
category: type of merchant or shopping category
amt: transaction amount
first: merchant first name
last: merchant last name
gender: merchant gender
street: merchant street address
city: merchant city
state: merchant state
zip: merchant postal code
lat: -
long: -
city_pop: population of merchant city
job: merchant job
dob: merchant date of birth
trans_num: transaction number
unix_time: -
merch_lat: -
merch_long: -
age: merchant age

Target Variable:
is_fraud: indicates whether the transaction was fraudulent (1 = fraud, 0 = not fraud)

Code & Implementation

Data preprocessing: handling missing values, encoding categorical features, scaling if needed

Model training: Logistic Regression, Random Forest, XGBoost

Model evaluation: metrics include Accuracy, Precision, Recall, F1 Score, ROC AUC

Flagged transactions saved to flagged_transactions.csv based on best threshold

Result
Best model chosen: XGBoost
Best threshold by F1 on test: 0.9076858
Accuracy: 0.9994
ROC AUC: 0.9808
Precision: 0.9583
Recall: 0.7041
F1 Score: 0.8118
Flagged transactions count: 72
Saved flagged transactions to flagged_transactions.csv

Observations:

XGBoost gave the best results with high accuracy and strong F1 score

High precision (0.9583) means most flagged transactions are actual frauds

Recall (0.7041) indicates some fraudulent transactions may be missed

Total 72 transactions were flagged for further review
