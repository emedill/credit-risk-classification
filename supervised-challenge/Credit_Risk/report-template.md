# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

The purpose of this analysis is to build a model that can identify the creditworthiness of borrowers. The goal is to create a reliable tool that can effectively distinguish between borrowers who are likely to repay their loans and those who might default.The financial data provided includes various information such as loan size, debt to income ratio, and total debt. In order to creat a machine learning model, it had to go through several steps. This includes separting the data into features and labels, splitting the data into training and testing datasets, and creating a logistic regression model. The purpose of that model is to predict the probability of an instance belonging to a particular class. After the predictions are computed, I then evaluted its performance by calculating the accuracy score through sklearn.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:

*Precision (0): The precision for class 0 is 1.00, meaning that when the model predicts class 0, it's always correct. 

*Recall (0): The recall for class 0 is 1.00, suggesting that there aren't any false negatives.

*F1-score (0): The F1-score is 1.00, indicating a perfect balance between precision and recall for this class.

*Support (0): The support for class 0 is 18759, which is the number of instances belonging to class 0 in the dataset.

*Precision (1): The precision for class 1 is 0.87, implying that it's correct approximately 87% of the time.

*Recall (1): The recall for class 1 is 0.89, meaning that the model correctly identifies around 89% of all instances of class 1.

*F1-score (1): The F1-score for class 1 is 0.88, representing the mean of precision and recall.

*Support (1): The support for class 1 is 625, which is the number of instances belonging to class 1 in the dataset.

* Overall Accuracy: The overall accuracy of the model is quite high at 99%

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

Based on the results of the logistic regression model, it has high accuracy and effectively classifies loan risk. There is a good balance between precision and recall for both classes, which is important for minimizing financial risks associated with lending to high-risk borrowers. I would recommend using this model for the company's lending decision process. However, like any model, it is important to occasionally monitor it since it has the potential to make incorrect predictions.