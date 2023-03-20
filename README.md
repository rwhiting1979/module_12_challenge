# Credit Risk Analysis Report

## Overview of the analysis
The purpose of this analysis is to train and evaluate logistic regression models using imbalanced classes. The credit risk dataset from a peer-to-peer lending services company is used for this analysis. The dataset contains historical lending activity, and we will build a model to identify the creditworthiness of borrowers.

Two versions of the dataset will be compared - one using the original dataset and another using the resampled data with the RandomOverSampler module from the imbalanced-learn library. For both cases, we will count the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.

## Results
Original Data Model
Balanced Accuracy Score: 0.9520479254722232
Precision Score:
Healthy Loans: 1.00
High-risk Loans: 0.85
Recall Score:
Healthy Loans: 0.99
High-risk Loans: 0.91
Resampled Data Model
Balanced Accuracy Score: 0.9936781215845847
Precision Score:
Healthy Loans: 1.00
High-risk Loans: 0.84
Recall Score:
Healthy Loans: 1.00
High-risk Loans: 0.99

## Summary
The logistic regression models trained on both the original and resampled data performed very well with high accuracy scores, precision, and recall scores. However, the model trained on resampled data performed better than the model trained on the original data.

The original data model had a balanced accuracy score of 0.952 while the resampled data model had a balanced accuracy score of 0.994, which is significantly higher. The resampled data model had a slightly lower precision score for high-risk loans compared to the original data model. However, the recall score for high-risk loans is much higher in the resampled data model, indicating that it is better at identifying high-risk loans.

Based on the analysis, we recommend using the resampled data model for identifying high-risk loans. This is because it has a significantly higher balanced accuracy score and higher recall score for high-risk loans compared to the original data model.
