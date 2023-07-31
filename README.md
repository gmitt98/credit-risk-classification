# credit-risk-classification

### Repo:

This repo contains a folder called Credit_Risk.
In this folder we have our juypter notebook used in the analysis, and the data used.
The analysis performed looks at different machine learning models to predict high vs low risk loans given various data about the loan and the customer.

### Languages & Libraries
- Python (3.9.12)
- Pandas
- Numpy
- SciKitLearn


# Module 12 Report

## Overview of the Analysis


* *Purpose*: develop models that can predict if a loan is likely to be high-risk or not
* *Data*: we used data that contained over 77k samples with the following information:
    * loan size
    * interest rate
    * borrower income
    * debt to income ratio
    * number of accounts
    * derogatory marks
    * total debt
    * loan status
* *Target*: We were trying to predict loan status, which is 0 for good and 1 for bad
* *Process*: We split the data into two data frame, and fed the data into sklearn modules then evaluated the outcome. We resampled the data and modeled again to see what changed.
* *Methods*: We used the following methods:
    * fit a logistic regression model with the *original data* split 80/20 train/test
    * evaluate this model

    * fit a logistic regression model with *resampled training data* with even data points between labels
    * evaluate this model
    * compare to the first model

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

|   | precision  | recall  | F1 score  | support  |
|---|---|---|---|---|
| label 0 | 1.00  | 1.00  | 1.00  | 15001  |
| label 1 | 0.86  | 0.91  | 0.88  | 507  |
| accuracy |   |   | 0.99  | 15508  |
| macro avg | 0.93  | 0.95  | 0.94  | 15508  |
| weighted avg | 0.99  | 0.9  | 0.99  | 15508  |


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.


|   | precision  | recall  | F1 score  | support  |
|---|---|---|---|---|
| label 0 | 1.00  | 0.99  | 1.00  | 15001  |
| label 1 | 0.85  | 0.99  | 0.92  | 507  |
| accuracy |   |   | 0.99  | 15508  |
| macro avg | 0.93  | 0.99  | 0.96  | 15508  |
| weighted avg | 1.00  | 0.99  | 0.99  | 15508  |

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
