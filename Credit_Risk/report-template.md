# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

The objective of this analysis was to develop a machine learning model capable of assessing credit risk using financial data. The dataset comprised details on borrowers' loan sizes, interest rates, incomes, debt-to-income ratios, account numbers, derogatory marks, and total debt. Our task was to predict loan_status, which is categorized as 0 (healthy loan) or 1 (high-risk loan). Notably, the data showed a significant imbalance with a predominance of 0s, posing a challenge in accurately predicting the less frequent high-risk loans.

Here’s a brief overview of our approach:
* Data preprocessing: We organized the data by separating it into features and labels and addressed the imbalances, which is crucial for building an effective model.
* Model training: We opted for logistic regression, a robust method for binary classification tasks.
* Model evaluation: We assessed the model’s performance by analyzing metrics such as accuracy, precision, and recall.


## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.

Logistic Regression Model:
* Accuracy: Achieved an impressive 99%.
* Precision: Reached 87% for high-risk loans and 100% for healthy loans.
* Recall: Successfully identified 89% of the high-risk loans and 100% of the low-risk ones.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

The logistic regression model excelled, particularly in accurately predicting healthy loans with high precision and recall. It also performed commendably in identifying high-risk loans, albeit with slightly lower precision. With an overall accuracy of 99% and balanced accuracy of 94%, this model is highly recommended for credit risk prediction.

The choice of model depends on specific priorities:
* If minimizing false negatives is a priority (i.e., ensuring high-risk loans are identified), focusing on enhancing recall for the 1s is crucial.
* If reducing false positives is more critical (i.e., avoiding incorrect classification of loans as high-risk), the model’s current performance is satisfactory.

With adjustments made to handle data imbalances through oversampling, the logistic regression model proves to be highly effective not only in identifying high-risk loans but also in confirming healthy ones, thus establishing itself as a robust tool for credit risk assessment within the lending industry.
