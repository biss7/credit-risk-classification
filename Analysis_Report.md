# Module 20 Analysis Report

## Overview of the Analysis

The purposes of this analysis is to create a logistic regression model to predict whether or not a loan will have a healthy status or high risk status based off of a variety of features. These features include the size of the loan, the interest rate, the borrower's income, the debt to income ratio, the number of accounts, if there are derogatory remarks, and the total debt of the borrower. 

The analysis takes historical data and splits it into two datasets: training and testing. The features and loan statuses of the training dataset are used to create the logistic regression model. The model is then applied to the features of the testing dataset to predict what the loan statuses will be. The results are then compared to the loan statuses of the testing data set to determine how well the model predicts the statuses.

RandomOverSampler is used to balance out the original training dataset so that there are an equal number of high risk loans to healthy loans. This new training dataset is used to create a new logistic regression model. The model is then applied to the features of the testing dataset to predict what the loan statuses will be. The results are then compared to teh loan statuses of the testing data set to determine how well the model predicts the statuses.

## Results

* Machine Learning Model 1:
  * Balance Accuracy Score: 0.944
  * Precision (Healthy): 1.00
  * Precision (High Risk): 0.87
  * Recall (Healthy): 1.00
  * Recall (High Risk): 0.89
  * Accuracy: 0.99

* Machine Learning Model 2:
  * Balance Accuracy Score: 0.996
  * Precision (Healthy): 1.00
  * Precision (High Risk): 0.87
  * Recall (Healthy): 1.00
  * Recall (High Risk): 1.00
  * Accuracy: 1.00

## Summary

Both models do well at making predictions on whether a loan will be high risk or healthy. However, the second model, where RandomOverSample was used on the training data, is more accurate (100%) than the first model (99%). In addition, the second model has a higher recall rate for high risk loans (100%) than the first model (89%). Therefore, the second model would be my recommended model.
