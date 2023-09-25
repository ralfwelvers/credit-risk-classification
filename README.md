credit-risk-classification

Ralf Welvers

September 25, 2023

The code can be found here:

Credit_Risk / credit_risk_classification.ipynb

The data used can be found here:

Credit_Risk / Resources / lending_data.csv

The Credit Risk Analysis Report can be found below.

## Overview of the Analysis

The purpose of the analysis is to determine if a specific dataset can be used to predict whether a new borrower will be a credit risk or not.
The dataset includes data such as loan size, dept to income ratio, borrower income, etc.
A logistic regression model was used. "y" was set to the “loan_status” column. Then "X" was set to the remaining columns.
Then the data was split the data into training and testing datasets by using train_test_split.
Then I created the predicted values for the testing and the training data.
Finally, a confusion matrix was created for the training and testing data along with classification reports for training and testing data.


## Results

Here's a break down of the evaluation metrics.

For Label 0:

* Precision: In the testing model, the precision for label 0 is 1.00, and in the training model, it's 1.00 as well. This means that when the model predicts label 0, it is almost always correct.
* Recall: In the testing model, the recall for label 0 is 1.00, and in the training model, it's 0.99. This indicates that the model captures almost all instances of label 0 in the testing set and the majority of instances in the training set.
* F1-score: The F1-score is a harmonic mean of precision and recall, and it is also high for label 0 in both testing and training models.

For Label 1:

* Precision: In the testing model, the precision for label 1 is 0.87, and in the training model, it's 0.85. This suggests that when the model predicts label 1, it is correct most of the time.
* Recall: In the testing model, the recall for label 1 is 0.89, and in the training model, it's 0.89 as well. This indicates that the model captures a substantial portion of instances of label 1 in both the testing and training sets.
* F1-score: The F1-score for label 1 is also relatively high, though slightly lower compared to label 0, in both testing and training models.


## Summary

In summary, the logistic regression model performs well for both label 0 and label 1. It achieves high precision, recall, and F1-scores for both classes in both the testing and training datasets. This suggests that the model is effective at making predictions for both classes, with only a slightly lower performance for label 1 compared to label 0.


