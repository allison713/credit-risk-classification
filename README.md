# credit-risk-classification

This project is an example of using Logistic Regression for Machine Learning to train a model to classify loans as healthy or unhealthy before processing.

I read csv data using pandas, then separated the labels from the features by manipulating a dataframe. 

In preparation for the analysis, the data was then scaled using a Standard Normal Distribution and split into a train and test group using sklearn.

I fit a Logistic Regression model and used it to predict the outcomes of the test data to analyze how well the model performed. 

At the beginning, it was noted that the data was extremely biased with 30 times more data in the healthy category, so I usesd Imbalanced Learning's Random Over Sampler to restructure the training data before trying Logistic Regression again. 

The model performed significantly better in recall, so there was less mislabeled data. 


Sources: 
Imbalanced Learn RandomOverSampler Documentation. https://imbalanced-learn.org/stable/references/generated/imblearn.over_sampling.RandomOverSampler.html#examples-using-imblearn-over-sampling-randomoversampler

Mathematical Equations for Accuracy, Precision, Recall: https://developers.google.com/machine-learning/crash-course/classification/precision-and-recall