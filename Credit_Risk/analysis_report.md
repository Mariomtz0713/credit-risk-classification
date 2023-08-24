# Report Analysis

## Background
The purpose of this analysis was to to use various methods to train and evaluate a model based on loan borrower risk. 

## Dataset
The lending data set consists of 77,536 data points and is split into training and testing sets. The X parameters were loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, and total debt. The Y parameter was the loan status.

## Predictions
Both models would be fed the X parameters to predict if a borrower would be low-risk with value of 0 or high-risk with a value of 1.

## Methods
The first method used the original unaltered data through the Logistic Regression model. The second method altered data to eliminate data imbalance with Random Over Sample module that was then implemented into the Logistic Regression model.

## Results

* Machine Learning Model 1: Original Data
  * Precision: 
    * 100% low-risk, 85% high-risk
  * Recall:
    * 99% low-risk,, 91% high-risk 
  * Balanced Accuracy Score: 99%

* Machine Learning Model 2: Resampled Data
  * Precision: 
    * 100% low-risk, 84% high-risk
  * Recall:
    * 99% low-risk,, 99% high-risk 
  * Balanced Accuracy Score: 99%

## Summary
Both models were very similar with having a balanced accuracy score of 99% respectively. However, I would recommended machine learning model 2 because its high-risk recall precision is at 99% compared to model 1's 91%.

An 8% high-risk recall difference is a lot mroe noticable to a 1% loss in high-risk's precision as classifiing low-risk when in reality a borrower is high-risk has a bigger impact on the company.
