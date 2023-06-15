# Credit Risk Classification
## Overview of the Analysis
* The purpose of this analysis is to evaluate two machine learning models to evaluate loan risk. 
* A dataset of historical lending activity from a peer-to-peer lending services company was used to identify the creditworthiness of borrowers.
* The variables that were used to predict creditworthiness of borrowers were the value counts of the loan status. The two loan statuses used were Healthy (0) and High-Risk (1)
* The Data was split into Training and Testing Sets by utilizing the train_test_split method 
* Two methods were used to analyze the Data:
	* A Logistic Regression Model was used with the original data 
	* A Logistic Regression Model was created with Over-Sampled Training Data. 

## Results
* Machine Learning Model 1: A Logistic Regression Model was used with the original data
  *  Balanced Accuracy Score: 95%
  * Precision Score: 0-100% and 1-85% As can be seen the model was able to predict healthy loans better than high-risk loans 
  * Recall Score: 0-99% and 1-91% As seen the model was able to correctly identify healthy loans better than high risk loans 

* Machine Learning Model 2: A Logistic Regression Model was created with Over-Sampled Training Data
    *  Balanced Accuracy Score: 99%
  * Precision Score: 0-100% and 1-85% As can be seen the model was able to predict healthy loans better than high-risk loans 
  * Recall Score: 0-99% and 1-91% As seen the model was able to correctly identify healthy loans better than high risk loans

## Summary

The oversampled model generated a balanced accuracy score of 99% which is higher than the original model. This model also does better at catching false negative and false positive scores for both health and high-risk loans. 
