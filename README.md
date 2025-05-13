# Loan Default Prediction Using Logistic Regression

## Overview of the Analysis
This analysis focuses on using a machine learning model—specifically logistic regression—to predict the likelihood that a loan will be repaid or defaulted on. The purpose of this analysis is to help financial institutions assess lending risk based on applicants' financial data.

The dataset (lending_data.csv) includes financial information such as the loan amount, interest rate and other attributes relevant to lending decisions. The target variable is loan_status, which indicates whether a loan was repaid (0) or not repaid (1).

The machine learning process followed these stages:

* Loaded and inspected the data using Pandas.
* Separated the data into features (independent variables) and the target (loan_status).
* Split the dataset into training and testing subsets using train_test_split.
* Trained a LogisticRegression model on the training data.
* Evaluated the model's performance using a confusion matrix and classification report.

## Results
Machine Learning Model 1: Logistic Regression

* Accuracy Score: 99.25%
* Precision: 99.39%
* Recall: 99.81%
* Specificity (True Negative Rate): 84.1%
* F1 Score: 99.60%

## Summary
The logistic regression model demonstrates excellent performance with high accuracy, precision, and recall. Based on these metrics:

* Recommendation: The logistic regression model is effective and should be considered for deployment in predicting loan repayment likelihood with similar datasets.

* Best Performing Metric: Recall (99.81%) is particularly strong, which is important when minimizing false negatives—i.e., when it's crucial not to miss potential defaulters.

* Contextual Importance: In the financial lending domain, predicting 1's (loan defaults) is more critical than predicting 0's, as failing to identify a defaulter poses a financial risk. This model’s high recall makes it especially valuable for that purpose.