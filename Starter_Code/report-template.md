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
      Overall the accuracy is high.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
