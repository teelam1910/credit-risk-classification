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

Accuracy scores, precision and recall scores of machine learning model.

* Machine Learning Model :
    * Description of Model Accuracy, Precision, and Recall scores.
        * For status 0 (healthy loans):
            - Precision: 1.00 (100%)
            - Recall: 0.99 (99%)
            - F1-score: 1.00 (100%)
        * For status 1 (high-risk loan)
            - Precision: 0.85 (85%)
            - Recall: 0.91 (91%)
            - F1-score: 0.88 (88%)


## Summary

Based on the data, the machine learning model demonstrates superior performance in predicting loan status 0 compared to status 1. Predictions for status 0 consistently achieve between 99-100% accuracy, indicating high precision. In contrast, predictions for status 1 exhibit a lower accuracy rate, with an F1-score of 88% and a recall of 91%. These metrics suggest that the model may not be optimal for training on high-risk loans.

Furthermore, an examination of the data revealed an imbalance between the two loan statuses. Upon inspecting the distribution of y values, it was observed that there were 75,036 instances of status 0 loans and only 2,500 instances of status 1 loans. This disparity likely contributed to the discrepancy in accuracy between the two loan types. To address this, the data for status 0 loans was reduced to 2,500 instances to align with status 1, aiming to balance the dataset. Although this approach involved dropping a substantial amount of data, it was undertaken for testing purposes without prior consultation with stakeholders.

Upon achieving a balanced dataset, notable improvements were observed in accuracy, precision, and recall scores for both loan statuses:

For status 0 (healthy loans):<br>
Precision: 0.99<br>
Recall: 1.00<br>
F1-score: 0.99<br>

For status 1 (high-risk loans):<br>
Precision: 1.00<br>
Recall: 0.99<br>
F1-score: 0.99<br>

Following data balancing, the accuracy for status 1 loans improved significantly, aligning with the accuracy levels of status 0 loans. While dropping data may not be ideal in practical applications, it notably enhanced the training model's performance in this instance.

Overall, despite the improvements after balancing the dataset, the model's accuracy still falls short for both loan statuses. Consequently, I would not recommend utilizing this training model without further refinement to enhance its accuracy across all loan status options. 

![concat line](https://github.com/teelam1910/credit-risk-classification/assets/132629216/a2d693bb-cc67-4bcb-a0b3-46d2c7520977)
![classification_report](https://github.com/teelam1910/credit-risk-classification/assets/132629216/f95567b2-38dc-4962-952f-11bcc1485c78)

