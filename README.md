# Practical Application III: Comparing Classifiers

For the detailed steps I used in this analysis, please refer to [Jupyter Notebook](https://github.com/losflo/ml-comparing-classifiers/blob/main/prompt_III.ipynb)

### Business Objective
To develop a classification model that predicts whether a client will subscribe to a term deposit. This model will be used to create marketing campaigns aimed at customers with a high probability of subscribing to a term deposit.

### Summary
The metric we used for scoring was accuracy. As this is a highly imbalanced data set using this may not be the best metric to base performance off of as 87% of the dataset belongs to one class of data. In order to more correctly identify the metric required the Business Objective would need to be more defined. Would the client want to air on the side of Misclassifying a Positive instance (Precision) or perfectly classifying the positive instances (Recall).

Based on this question as we selected accuracy as our metric. I would select Decision Tree Classifier as the model to deploy in Production. As this has the best accuracy, and the fastest train time. I found the most influential features to be month, contact, and age using `permutation_importance`

