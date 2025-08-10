# Multiple Models
This repository contains different strategies for using multiple models, such as Growing Ensembles , Pruning Ensembles, Hard Voting, Soft Voting, Voting for Regression, OneVsRest, OneVsOne... .
## Voting
The weighted ensemble approach averages the predictions of several models, adjusting their contribution based on their performance through voting.

### Hard Voting (Classification)
- The voting process selects the class that receives the majority of votes from the involved classifiers.

### Soft Voting (Classification)
- The probabilities of each class from the classifiers are averaged, and the class with the highest average probability is chosen as the final prediction.

### Voting for Regression
- The Voting Regressor in regression averages the continuous values of the model predictions. There is no hard or soft voting like in classification.

## Ensemble Pruning
- It is a method that starts by including all possible elements in the ensemble and progressively removes them until no further improvement can be achieved. This elimination can be performed greedily, removing one element at a time only if its removal improves the ensemble’s performance.

## OneVsRest
The approach consists of transforming a multi-class classification problem into several binary classification problems by training a binary classifier for each class. To predict the class of a new instance, the probability or score of each classifier is calculated, and the class with the highest score is selected as the prediction.

## OneVsOne
It divides a multi-class classification into a binary classification problem for each pair of classes. Since the model is trained for each pair of classes, it can better handle class imbalances between different pairs, which can improve accuracy and the handling of minority classes.

## Error-Correcting Output Codes (ECOC)
Error-Correcting Output Codes (ECOC) is a strategy for solving multiclass classification problems by decomposing them into multiple binary classification tasks. Each class is assigned a unique binary code (a row in a coding matrix), and a binary classifier is trained for each column of the code. During prediction, the combined output of the classifiers is compared to the class codes using a distance measure (e.g., Hamming distance) to identify the most likely class. ECOC improves robustness against errors from individual classifiers by leveraging principles from error-correcting codes.


