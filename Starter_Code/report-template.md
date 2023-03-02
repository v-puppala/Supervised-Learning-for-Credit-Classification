# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

Since the machine learning models we utilize directly inform our decision making and generate insights, it's important to assess model performance before accepting the generated results. The classic adage "garbage in, garbage out" encapsulates the necessesity to analyze the model performance. This is because the quality of the predictions from the model inference is highly dependent upon the quality of training and how well the trained classifier/regressor generalizes.

The problem statement is to classify creditholders into two groups: high risk and healthy, based on several features such as loan size, interest rate, borrowing rate, etc. The output of the model is one of two scores that measure borrowers' creditworthiness.

As part of the analysis, we oversaw a traditional ml workflow. First we extracted our sample data from a dataframe exploring historical lending activity from a peer-to-peer lending company that contains consumer data and their credit statuses. Then we applied applied a standard 60/40 training-testing split to our dataset, prior to appplying standard normalization scalar to our training and inference groups,to ensure that each feature is weighed equally. Then we applied two models to the scaled sets, both logistic regressors, one with resampling and one without.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
      Overall the accuracy is high.  However, class 0/the healthy group ( has a notably higher precision and recall than for class 1/the high risk group. Moreover, the support for class 1 is 619 while the support for class 0 is significantly higher (18765). This along with the fact that class 0 has near perfect percision/recall while class 1 has Precision/recall values in the .80  and early 0.90 range, indicate that most of the incorrectly classified labels belong to class 0 and not class 1. Overall there are few mistakes made, relative to the overall number of classifications made, but of the mistakes made, is is apparent that the high risk group accuracy rate is lower relative to its support.s 
      



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores
  
  Overall the accuracy and precision are high for both classes. However, the precision is still higher (.99) for class 0 than for class 1 (0.84).

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
Overall the resampled model is better, as it improves the recall for class 1. 

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )


It depends on what we prioritize as more detrimental. Even with the improved model (model 2), we still encounter the problem where we wrongly classify  with high creditworthiness to the group less likely to pay their credit. 

If you do not recommend any of the models, please justify your reasoning.
