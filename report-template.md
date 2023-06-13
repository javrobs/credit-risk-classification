# Module Report 

## Overview 

* The purpose of this analysis is to take a large dataset of customer loans and the current flagging system to create a model that can flag loans as high-risk or healthy for a bank.
* The data included the amount of the loan required, the debt of the customer, their income and other financial information. 
* One problem with the dataset is that the proportion of the risk level is not equal, meaning that the models will have more examples of healthy loans than high-risk loans, which might affect it making it more likely that the model will assume loans are on the healthy side.
* One solution we implemented to overcome that issue is the usage of random oversampling, which essentially duplicates existing values of a 
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
    


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
