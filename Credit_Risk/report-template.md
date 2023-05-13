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

* Random Over Sampled Logistic Regression Model:
  * Precision: 99.98% of applications labeled as healthy by the model were known to be healthy. However, only 84.1% of the applications labeled as high risk are known to be high risk. This was worse than before random sampling. I'm not sure why.
  * Recall: 0.6% of applications known to be healthy were mislabeled and 0.6% of applications known to be high risk were mislabeled. This showed a marked improvement after resampling. 

## Summary

It would be better for the company for the model selected to over predict healthy loans if we are going to then process the requests by hand. This ensures that healthy applicants are processed and unhealthy ones can then be removed. If our model over predicts unhealthy loans, we may reject loan applications before a human has a chance to review the information. 

However, if we are going to automatically accept loan applications based on classification as healthy, then we should over predict unhealthy loans so that a human can then filter through the applications and find the false negatives.


* Overall I think that the resampled data model predicted better as fewer of the loans were individually misclassified.
