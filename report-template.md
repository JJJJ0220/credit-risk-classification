# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
The primary goal of this analysis was to apply machine learning models to assess credit risk accurately. This involved predicting the likelihood of borrowers defaulting based on their financial histories.
* Explain what financial information the data was on, and what you needed to predict.
The dataset comprised various financial attributes of borrowers. Key variables included credit scores, loan amounts, debt-to-income ratios, and payment histories. Our target variable was a binary indicator of credit risk (e.g., 'high risk' vs. 'low risk').
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
Data Preprocessing: Cleaning data, handling missing values, and encoding categorical variables.
Feature Selection: Identifying the most relevant variables for predicting credit risk.
Model Training and Testing: Splitting the data into training and testing sets, and applying different machine learning models.
Evaluation: Assessing each model's performance using various metrics.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
We employed models like Logistic Regression, supplemented by resampling methods to address imbalances in the dataset.


In this task, we're creating a system to determine if people borrowing money are likely to pay it back. We'll use various pieces of information like the amount of the loan, the interest rate, the borrower's income, their debt compared to their income, the number of their bank accounts, any past payment issues, and their total debt. Our goal is to predict something called 'value_counts'.

We'll start by loading a file named "lending_data.csv" into a program called Pandas, which helps us manage data. Then, we'll divide this data into two groups: one for training our model and one for testing it.

We'll use a method called Logistic Regression to train our model. This will help us predict the 'value_counts' based on the information we have about the borrowers.



## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
     precision    recall  f1-score   support

           0       1.00      1.00      1.00     18763
           1       0.87      0.85      0.86       621

    accuracy                           0.99     19384
   macro avg       0.93      0.92      0.93     19384
weighted avg       0.99      0.99      0.99     19384


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
     precision    recall  f1-score   support

           0       1.00      0.99      1.00     18763
           1       0.87      0.99      0.93       621

    accuracy                           0.99     19384
   macro avg       0.93      0.99      0.96     19384
weighted avg       1.00      0.99      1.00     19384

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
In conclusion, model 2 performed better with higher accuracy . For instance, if predicting '1's (high-risk borrowers) is more critical, a model with higher recall for '1's might be preferred. Conversely, if overall accuracy is paramount, the model with the highest balanced accuracy score would be ideal.

If you do not recommend any of the models, please justify your reasoning.


The second model we created is a bit more accurate than the first one. 
