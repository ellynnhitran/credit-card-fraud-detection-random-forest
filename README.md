# credit-card-fraud-detection

# Project Overview
This project aims to develop a robust and accurate credit card fraud detection system using a Random Forest classifier. The dataset used in this project contains transactional data, with features that describe the transactions and labels indicating whether a transaction is fraudulent.

# Dataset
The dataset is divided into two main files:
- fraudTrain.csv: Training dataset containing labeled transactional data.
- fraudTest.csv: Testing dataset containing labeled transactional data.

# Key Features:
merchant: Merchant name
category: Transaction category
amount: Transaction amount
cc_num: Credit card number
first, last: Cardholder's first and last name
gender: Cardholder's gender
street, city, state, zip: Cardholder's address
lat, long: Cardholder's latitude and longitude
city_pop: Population of the city
job: Cardholder's job
dob: Cardholder's date of birth
trans_num: Transaction number
unix_time: Transaction time in Unix format
merch_lat, merch_long: Merchant's latitude and longitude
is_fraud: Label indicating if the transaction is fraudulent (1) or not (0)

# Steps to reproduce
1. Data Preprocessing
- Collect Data
- Prepare the Data
 + Clean: Address any missing or corrupt data.
 + Normalize: Normalize numerical data with Standard Scaler.
 + Encode: Transform categorical data into numeric formats through one-hot encoding for categorical features.
 + Feature Engineering: Create new feature "hour of the day" to enhance patterns analysis
   
2. Exploratory Data Analysis
- Spending Category VS Fraud
- Gender VS Fraud
- Age VS Fraud
- State VS Fraud
- City VS Fraud
- Job VS Fraud
- Credit Card Number/Holder with the Most Fraud
- Transaction Amount VS Fraud
- Cyclicality of Credit Card Fraud
  
3. Train the Model: Configure and train a logistic regression model using the training data.
   
4.  Evaluate the Model: Assess the model with the testing data using metrics suited for imbalance, such as precision, recall, and F1-score.
   
5. Model Optimization and Tuning
- Regularization Techniques: Experiment with different regularization techniques.
- Adjust Decision Threshold: Adjust the threshold value to balance between precision and recall.
  
6. Re-evaluate the Optimized Model
   
7. Deploy model
