# Module Report 

## Overview 

* The purpose of this analysis is to take a large dataset of customer loans and the current flagging system to create a model that can flag loans as high-risk or healthy for a bank.
* The data included the amount of the loan required, the debt of the customer, their income and other financial information. 
* One problem with the dataset is that the proportion of the risk level is not equal, meaning that the models will have more examples of healthy loans than high-risk loans, which might affect it making it more likely that the model will assume loans are on the healthy side.
* One solution we implemented to overcome that issue is the usage of random oversampling, which essentially duplicates existing values of the minority group, in this case high-risk loans as well as randomly take out 

## Results
* Classic Logistic Regression
  * Accuracy = 94.43%
  * Precision:
      * Healthy = 99.64% - Predicted "Healthy" are categorized correctly 
      * High-risk = 87.46% - Predicted "High-risk" are categorized correctly
  * Recall:
      * Healthy-risk = 99.57% - Real "Healthy" are categorized correctly
      * High-risk = 89.28% - Real "High-risk" are categorized correctly

* Logistic Regression with Random Oversampling
  * Accuracy = 99.6%
  * Precision:
      * Healthy = 99.99% - Predicted "Healthy" are categorized correctly 
      * High-risk = 87.25% - Predicted "High-risk" are categorized correctly
  * Recall:
      * Healthy-risk = 99.51% - Real "Healthy" are categorized correctly
      * High-risk = 99.68% - Real "High-risk" are categorized correctly
 

## Summary

Using Random Oversampling gave the model a better ability to put the accurately flag the high-risk loans from 89.28% (About 1 in 9 undetected) to 99.68% (About 1 in 312 undetected). The improvement in recall for high-risk loans makes this model superior and a lower risk to implement.
  
Flagging the high-risk loans is the most critical part of the model, since we prefer denying a loan to someone who might have payed back versus loaning and having someone not pay.
  
A precision of 87% for high-risk loans might seem low but assuming the distribution of the data represents the real world, only 3.33% of loans were dangerous, while the model flags 3.82%.
  
**For these reasons, the oversampled model is superior and could be implemented to accurately classify the type of loan.**