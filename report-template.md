# Credit Risk Classification Report

## Overview of the Analysis

The purpose of this analysis is to develop a predictive model for assessing loan risk using machine learning modeling. The dataset included financial variables such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, and derogatory marks. These features were used to train the model to predict loan status, where '0' represented healthy loans and '1' represented high-risk loans.

Exploratory analysis of the loan_status variable revealed its distribution, later aiding in discovering and understanding dataset imbalance and selecting appropriate evaluation metrics. The machine learning process involved splitting the data, into training and testing datasets, and ensuring the random_state as 1. Algorithms, including logistic regression, train-test split evaluation from sklearn.model_selection were utilized.

When creating a Logistic Regression Model with the Original Data, the LogisticRegression method was used. To evaluate the model, the following steps were taken:

- Generated predictions using X_test data.
- Constructed a confusion matrix to visualize model predictions compared to actual loan statuses.
- Printed the classification report, providing a comprehensive overview of the model's performance, including precision, recall, and F1-score for each class.
  
These evaluation techniques provided insights into the model's effectiveness in accurately classifying loan statuses, aiding in determining its practical utility in real-world scenarios.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
