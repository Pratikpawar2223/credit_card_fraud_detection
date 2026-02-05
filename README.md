# Credit-Card-Fraud-Detection

## Table of Contents
- Data Set
- Result

---

## Data Set
This dataset contains information about credit card transactions and helps identify whether a transaction is fraudulent or not.

The dataset contains a total of **22 features**.

### Features Description
- **trans_date_trans_time** – Transaction date and time  
- **cc_num** – Credit card number  
- **merchant** – Merchant name  
- **category** – Type of merchant category  
- **amt** – Transaction amount  
- **first** – Customer first name  
- **last** – Customer last name  
- **gender** – Customer gender  
- **street** – Customer street address  
- **city** – Customer city  
- **state** – Customer state  
- **zip** – Customer postal code  
- **lat** – Customer latitude  
- **long** – Customer longitude  
- **city_pop** – Population of the customer’s city  
- **job** – Customer job  
- **dob** – Customer date of birth  
- **trans_num** – Transaction number  
- **unix_time** – Transaction time in Unix format  
- **merch_lat** – Merchant latitude  
- **merch_long** – Merchant longitude  
- **age** – Customer age  

### Target Variable
- **is_fraud** – Indicates whether the transaction is fraudulent or not  
  - `1` → Fraud  
  - `0` → Not Fraud  

---

## Result
- **Logistic Regression**: Accuracy = **0.92**
- **Random Forest Classifier**: Accuracy = **0.99**
- **Support Vector Machine (SVM)**: Not evaluated due to high computation time
