# Credit Risk Classification

## Overview of the Analysis

The purpose of this analysis was to decide if a Logistical Regression model using the historical lending activity from a peer-to-peer lending service company appropriately identified the creditworthiness of borrowers. 

The data included features of loan size, interest rate, borrower income, number of accounts, derogatory marks, and total debt. The prediction target was the loan status – either healthy (75,036 cases) or high risk (2500 cases). 

As part of this analysis, the data was separated into target and features and then split with the sklearn module’s train_test_split. Then with the sklearn module’s LogisticRegression, the model was instantiated. Following that, the model was predicted and tested with a confusion matrix and a classification report.

## Results

* Accuracy: 99%
* Healthy Loans
	* Precision: 100%
	* Recall: 100%
* High-Risk Loans
	* Precision: 87%
	* Recall: 89%


## Summary

I would recommend the logistic model as an appropriate model for it performed well overall. While there is still 11% of high-risk loans that slipped past, that is only 275 loans out of 75,286 (or 0.3%) with a recall error on their loan status with this model. The only criticism I have for the model is more of a curiosity about the feature importance that using the Random Forest model would provide. If the company was likewise curious, I’d recommend testing it. If it resulted in less accuracy, precision, and recall, then feature importance would not be worth the effectiveness of the logistic regression model.
