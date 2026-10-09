# Random Forest: Hyperparameter Selection with the OOB Score

This section of the data-centric-ml repository focuses on the study and practical application of Random Forest techniques within the field of Machine Learning.

It brings together a collection of experiments, methodologies, and strategies for:

- Selecting Random Forest hyperparameters
- Using the out-of-bag (OOB) score as an alternative to cross-validation
- Evaluating predictive performance and generalization
- Comparing the computational cost of each selection strategy

The goal is to explore the OOB score from a practical perspective, comparing it with GridSearchCV in regression and classification problems.

## 01 OOB Score vs GridSearchCV: Regression
Comparison of GridSearchCV and the OOB score (default and custom metric) for selecting Random Forest hyperparameters in a regression problem, including selection time and test performance.

## 02 OOB Score vs GridSearchCV: Classification
Comparison of GridSearchCV and the OOB score (default and custom metric) for selecting Random Forest hyperparameters in a multiclass problem with imbalanced classes, using macro F1 as the evaluation metric.
