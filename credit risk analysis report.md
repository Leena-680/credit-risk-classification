# Module 12 Report 

## Overview of the Analysis

The purpose of the analysis is to train and evaluate a model on loan risk. The dataset used for the project is historical lending activity from a peer-to-peer lending services company. Variables in the dataset included loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and loan status.

A logistic regression model will be used to identify the credit worthiness of borrowers as either high-risk (unhealthy loan/defaulting) or low-risk (healthy loan).

Loan status is the dependent variable (y). Loans are identified as either defaulting (1) or healthy (0). The remaining variables are used as predictors (x). 

## Results

* logistic regression model:
  * The input file has 77536 records. The input data is split into training data and test data. Training data is used to generate logical regression model. The accuracy of this model is tested by generating confusion matrix and classification report.
  * Our balanced accuracy score is 94%. The balanced accuracy score takes into account the sensitivity (true positive rate) and the specificity (true negative rate). The balanced accuracy score is measures the performance of our model, especially with imbalanced datasets. In our dataset, we have 77536 loans that were rejected, but only 2500 that were accepted. Since our data is imbalanced, the balanced accuracy score serves as a good metric for the performance of our model.
  * Another measure of performance for our model is accuracy. The model's accuracy score is 99%, which means that the model correctly predicted 99% of all loans in the dataset.
  * Based on the confusion matrix, the model accurately accepted 18679 healthy loans and rejected 558 high-risk loans. However, the model also incorrectly rejected 80 healthy loans and incorrectly accepted 67 high-risk loans.
  * The F1 score is a weighted average of the precision and recall scores. Our model's F1 score is 88%.
  

## Summary

Logical regression model performs well in predicting healthy loans, however, has a lower performance for predicting high-risk loans. In addition, this could lead to a higher rate of false positives or false negatives.
