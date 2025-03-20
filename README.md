Credit risk classification
Overview
In this challenge, we utilize various machine learning techniques to train and evaluate a Logistic Regression model for predicting loan risk. The goal is to determine whether a loan is healthy (0) or high-risk (1) based on historical lending activity. The dataset comes from a peer-to-peer lending services company, providing valuable insights into borrower creditworthiness.

Dataset
The dataset consists of 77,536 loans with the following features:

loan_size – The amount of the loan
interest_rate – The interest rate assigned to the loan
borrower_income – The borrower's annual income
debt_to_income – The borrower’s debt-to-income ratio
number_of_accounts – The total number of accounts held by the borrower
derogatory_marks – Any negative marks on the borrower’s credit history
total_debt – The total debt held by the borrower
loan_status – The target variable indicating whether the loan is healthy (0) or high-risk (1)
Machine Learning Process
The model development follows a structured machine learning workflow:

Data Preparation – Import the dataset, clean the data, and establish a DataFrame.
Feature and Label Separation – Define loan_status as the label (target variable) and use the remaining columns as features.
Train-Test Split – Use train_test_split to divide the dataset into training and testing subsets.
Model Selection – Implement a Logistic Regression model using sklearn.
Model Training – Fit the model using the training dataset.
Predictions – Use the trained model to make predictions on the test dataset.
Model Evaluation – Assess performance using metrics such as:
Balanced Accuracy Score
Confusion Matrix
Classification Report
