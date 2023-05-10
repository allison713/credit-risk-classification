# Module 12 Report Template

## Overview of the Analysis

The purpose of this analysis is to create a model, based on current loan customers, that can predict whether a new customer is a high risk or healthy borrower by analyzing the following borrower features: loan size, interest rate, income, debt to income ratio, number of open accounts, derogatory marks, and total debt.

The prior customer data used to train the model included 75036 healthy loan applications and 2500 high risk loan applications.

When using a Logistic Regression model to predict the riskiness of a loan application, the model was 99% accurate, but has bias toward healthy loan applications because of the bias in the training data. 

## Results

* Logistic Regression Model:
  * Precision: 99.7% of applications labeled as healthy by the model were known to be healthy. However, only 84.7% of the applications labeled as high risk are known to be high risk. This indicates that some healthy loan applications are classified as high risk.
  * Recall: 1% of applications known to be healthy were mislabeled and 9% of applications known to be high risk were mislabeled.
  * Accuracy: Overall the model was 99% accurate, but this may be skewed by the extremely high precision in the healthy predictions which are biased due to bias in the training data.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
