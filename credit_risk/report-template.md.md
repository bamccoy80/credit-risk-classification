# Module 20 Report Template

## Overview of the Analysis

* **Purpose of the analysis** - The objective of this analysis is to evaluate whether the Logistic Regression machine learning model can more accurately predict healthy loans and high-risk loans using the original dataset or a resampled dataset with an increased minority class size.
	* **The dataset** - The dataset for this analysis comprises information on 77,536 loans. It includes columns for **loan_size, interest_rate, borrower_income, debt-to-income ratio, number_of_accounts, derogatory_marks, total_debt,** and **loan_status**. The target variable for prediction is **loan_status**, while the remaining columns serve as features to train the model and generate predictions.
* **Stages of the Machine Learning Process** - The stages of the machine learing process are very scripted. If followed in order, they provide you with an accurate assessment of the model's ability to make predictions.  The stages of the machine learning process are as follows: 
	- Prepare the data - Import the file, establish the DataFrame, evaluate the columns and features.
	- Separate the data into features and labels- The labels are what you are attempting to predict, is the status of the loan healthy (0) or high-risk (1).  The features are all of the remaining data you will use to train and test the model. 
	- Use the train-test_split function to separate the features and labels data into training and testing datasets. 
	- Import the machine learning model from the library - In this instance, we will be importing LogisticRegression from SKlearn.
	- Instantiate the model. 
	- Fit the model using the training data.
	- Use the model to make predictions using the features test data. 
	- Evaluate the predictions- Evaluations are done by calculating and comparing metrics like accuracy score, a confusion matrix, and a classification report.  
* **Machine Learning Methods Utilized** - 
The primary model used in this analysis is:
	- LogisticRegression model from SKLearn

Supporting functions used in this analysis are
-    train_test_split form SKLearn
		
Models are evaluated using the follwing functions:
		-	confusion_matrix from SKLearn
		-	classification report form SKlearn


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model - Logistic Regression:
  * **Accuracy Score** 99% 
  * **Precision Score** 
	  * Class 0 (Healthy Loans): 100% 
	  * Class 1 (High-risk Loans): 85%
  * **Recall Scores**
	  *  Class 0 (Healthy Loans): 99% 
	  * Class 1 (High-risk Loans): 91%

## Summary


The model does a great job in using the original data to predicting the value of hte healthy laons. Precision was 100% and recall was 99%.

Logistic Regression model does well for predicting the values of high risks loans, but not the healthy loans. Precision is 84% and recall is 94%.

Based on the analysis, the Logistic Regression model demonstrates strong predictive performance in distinguishing between healthy loans and high-risk loans, given the selected features used for training. The evaluation metrics, such as accuracy score, confusion matrix, and classification report, indicate that the model effectively classifies both loan categories.
