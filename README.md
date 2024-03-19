# Challenge 20 - Supervised Learning

## Overview of the Analysis

The purpose of this analysis was to use various techniques to train and evaluate a model based on credit risk, for which a dataset of historical credit activity from a peer-to-peer lending company was used to create a model that can identify borrower solvency.
First, the data was divided into training and testing sets. Then, a logistic regression model was created with the original data.



## Results

* A value of 0 in the 'loan_status' column means the loan is in good standing, of which there are 18759 entries, and a value of 1 means the loan has a high risk of default, with 625 entries used. Therefore, the model is trained to detect healthy loans more accurately compared to high-risk loans.

* The model has an accuracy of 99%, meaning it correctly predicts 99% of all instances in the dataset.
In the macro avg, precision, recall, and F1-score metrics show that for healthy loans and high-risk loans, they are averaged and displayed as 0.94. This means that on average, the model performs well for both classes.

* Finally, the weighted avg weighs according to the number of instances of each class and is averaged. The result is 0.99, suggesting a very solid and balanced performance in the dataset.


|              | Precision |  Recall  | F1-Score | Support |
|--------------|-----------|----------|----------|---------|
| Healthy Loan |   1.00    |   1.00   |   1.00   |  18759  |
| High-risk Loan | 0.87    |   0.89   |   0.88   |   625   |
|--------------|-----------|----------|----------|---------|
| Accuracy     |           |          |   0.99   |  19384  |
| Macro Avg    |   0.94    |   0.94   |   0.94   |  19384  |
| Weighted Avg |   0.99    |   0.99   |   0.99   |  19384  |



## Summary

The prediction of Healthy Loan has a precision of 100%; on the other hand, the prediction of High-risk Loan has a precision of 87%.

From the provided dataset of High-risk Loan, 89% of the data was correctly identified. The F1-score is 0.88, which means few positive instances are classified incorrectly as negative.

The Healthy Loan(0) class performance better thank High-risk Loan(1); therefore, it 's highly recommended to use this prediction model.


