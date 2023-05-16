# Credit Risk Classification Report

## Overview of the Analysis

This analysis uses historical lending data from a peer-to-peer service to construct and compare two logistic regression models for assessing borrower creditworthiness. The models, built on data points such as loan size, interest rate, income, and debt ratios, predict loan statuses as '0' (healthy) or '1' (high-risk). The machine learning process involves splitting the data, fitting and evaluating models with original and resampled (via RandomOverSampler) data based on accuracy, precision, recall, and F1 scores. The aim is to enhance loan risk prediction accuracy.

## Results

*Machine Learning Model 1 Scores*
* __Overall Accuracy:__ 99%
* __Low Risk Loans__
  * __Precision:__ 100%
  * __Recall:__ 100%
* __High Risk Loans__
  * __Precision:__ 87%
  * __Recall:__ 89%

*Machine Learning Model 2 Scores*
* __Overall Accuracy:__ 99%
* __Low Risk Loans__
  * __Precision:__ 99%
  * __Recall:__ 99%
* __High Risk Loans__
  * __Precision:__ 99%
  * __Recall:__ 99%

## Summary

*Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:*

The performance of a machine learning model should align with the specific problem the client is trying to solve. In the context of credit risk assessment, prioritizing the accurate prediction of high-risk loans would likely be more important to clients, as they represent potential financial losses.

Model 1 shows perfect performance (100% precision and recall) for low-risk loans but lower performance (87% precision, 89% recall) for high-risk loans. While these high-risk scores are good, they might not be optimal for a context where minimizing high-risk loan misclassification is crucial.

Model 2, on the other hand, shows near-perfect performance across both loan categories with 99% precision and recall. Its high-risk loan prediction performance is noticeably better than Model 1.

Based on these results, if the main goal is to minimize potential financial losses by accurately identifying high-risk loans, Model 2 would be the more suitable choice due to its superior performance in predicting high-risk loans.

However, it's important to remember that every model has its trade-offs. Even though Model 2 appears to perform better overall, it might be slightly less precise in identifying low-risk loans than Model 1. If the client wants to prioritize identifying low-risk loans (e.g., to scale up operations or focus on customer acquisition), then Model 1 could be the better choice.

In sum, Model 2 is recommended for its balanced, near-perfect performance across both loan categories, particularly if the focus is on accurately predicting high-risk loans to minimize financial losses.