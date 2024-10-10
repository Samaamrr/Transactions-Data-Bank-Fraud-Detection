# Transactions-Data-Bank-Fraud-Detection
# Fraud Detection Model: Bank Transactions Data
# Project Overview
This project focuses on detecting fraudulent transactions using machine learning techniques. The dataset contains over 1 million transactions, each labeled as either fraudulent or non-fraudulent. Our goal was to analyze the dataset, preprocess the data, and build a machine learning model to predict whether future transactions will be fraudulent.

# Table of Contents
Dataset Description
Mission
Exploratory Data Analysis (EDA)
Data Preprocessing
Feature Engineering
Modeling
Evaluation Metrics
Conclusion
# Dataset Description
The dataset used in this project contains the following columns:

Date: The date of the transaction.
nameOrig: Unique identifier for the originating account.
amount: The transaction amount.
oldbalanceOrg: Balance before the transaction for the originating account.
newbalanceOrig: Balance after the transaction for the originating account.
City: The city where the transaction took place.
type: The type of transaction (e.g., TRANSFER, CASH_IN).
Card Type: The type of card used (e.g., Gold, Platinum, Silver).
Exp Type: Expense type category (e.g., Fuel, Food, Entertainment).
Gender: Gender of the account holder.
isFraud: Fraud label (1 = fraud, 0 = no fraud).
# Mission
The main objectives of this project are:

Perform data analysis to uncover trends and patterns in fraudulent vs. non-fraudulent transactions.
Build a predictive machine learning model to classify whether a transaction is fraudulent based on available features.
# Exploratory Data Analysis
We explored the dataset to uncover trends and gain insight into how fraudulent transactions differ from legitimate ones. Some key findings include:

Fraud Distribution: Visualized the percentage of fraud in the dataset. Fraud makes up around 16.8% of the transactions.
Transaction Trends: Analyzed how transaction amounts, types, and other factors correlate with fraudulent activity.
Visualizations:
Line plots showing transaction amounts over time.
Bar charts for transaction types, card types, and expense categories, split by fraud status.
# Data Preprocessing
Data Cleaning:
No missing values or duplicates were found in the dataset.
Converted the Date column to a proper datetime format.
Feature Selection:
Separated numeric and categorical columns for further preprocessing and analysis.
Feature Engineering
Date Features: Extracted day, month, and year from the Date column to create additional features for the model.
Drop Date Column: After extracting useful date features, we removed the original Date column.
# Modeling
We used classification algorithms to predict whether a transaction is fraudulent. The process included:

Feature Selection: Separated numerical and categorical columns for more effective modeling.
Training the Model: Trained a machine learning model using the processed data.
Tested different algorithms (e.g., Logistic Regression, Decision Trees) to find the most accurate model.
Evaluation: We evaluated the models using standard metrics like accuracy, precision, recall, and F1-score to ensure high fraud detection rates without too many false positives.
# Evaluation Metrics
We focused on the following metrics to evaluate the performance of our model:

Accuracy: Measures overall performance.
Precision: Measures the accuracy of fraud predictions (i.e., how many predicted frauds are actually fraud).
Recall: Measures how well the model detects fraud cases (i.e., out of all actual fraud cases, how many did the model correctly identify).
F1-Score: The harmonic mean of precision and recall, giving a balanced measure of model performance.
# Conclusion
This project successfully achieved its goals of fraud detection through machine learning. Our model can predict fraudulent transactions based on various features such as transaction amount, transaction type, card type, and more. This solution provides a valuable tool for banks to reduce fraud-related losses by flagging suspicious transactions in real-time.

# Future Enhancements
Further tuning and testing of different machine learning algorithms to improve prediction accuracy.
Incorporating additional features such as geolocation data or external transaction metadata to enhance model performance.
# How to Use
Install the necessary dependencies listed.
Load the dataset (Fraud.csv).
Run the notebook to see the data analysis, model training, and evaluation.
