# Basic Machine Learnining Projects
Linear Regression
Linear regression is a statistical technique that seeks to establish a linear relationship between a
dependent variable (Y) and one or multiple independent variables (X), by minimizing the sum of
squared differences between actual Y values and the values predicted by a linear equation. It aims
to estimate the coefficients (slope and intercept) of the linear equation, enabling prediction and
interpretation of the dependent variable’s variations based on changes in the independent variables.
For this assignment,
1. Split the dataset into 50% for training, 30% for validation and 20% for testing. Normalize/Regularize data if necessary. Encode categorical variables using appropriate encoding
method if necessary.
2. Formulate a linear regression model between the observations x
(i)
j
and target parameter
y
(i)
.
y
(i) = θ0 +
X
j
θj ∗ x
(i)
j
(1)
3. Use the mean squared error loss function to fit the 2 following models.
4. For the first model use the analytic solution as discussed in class. Report the R-squared
and RMSE score for the test set after training the model.
5. While for the second model use the an iterative solution via gradient ascent. Use 3 different learning rates- 0.01, 0.001 and 0.0001. Plot the Loss function for the training set and
validation set at each iteration. Finally report the R-squared and RMSE score for test set.

Logistic Regression
Logistic regression is a statistical method used for binary classification. It models the probability
of an event occurring by fitting a logistic curve to data, assigning values between 0 and 1. It’s a
vital tool for predicting outcomes like yes/no or true/false in various fields.
For this assignment,
1. Split the dataset into 50% for training, 30% for validation and 20% for testing. Normalize/Regularize data if necessary. Encode categorical variables using appropriate encoding
method if necessary.
2. Implement a standard Logistic Regression Classifier as discussed in class. Do NOT
use scikit-learn for this part.
2
3. Report the mean accuracy, precision and recall for the class 1(good)for the classifiers.
You may or may not use the scikit-learn implementations for computing these metrics.


Decision Trees 
Decision trees are graphical models that make decisions based on conditions, branching into outcomes or actions. They represent choices in a tree-like structure, aiding in classification or regression tasks by recursively partitioning data based on features, enabling interpretable and effective
decision-making.
For this assignment,
1. Split the dataset into 80% for training and 20% for testing. Normalize/Regularize data if
necessary. Encode categorical variables using appropriate encoding method if necessary.
2. Implement the standard ID3 Decision tree algorithm as discussed in class,using Information Gain to choose which attribute to split at eachpoint. Stop splitting a node if it has less
than 10 data points. Do NOT use scikit-learn for this part.
3. Perform reduced error pruning operation over the tree obtained in (2). Plot a graph
showing the variation in test accuracy with varying depths. Print the pruned tree obtained
in hierarchical fashion with the attributes clearly shown at each level.
4. Report the mean macro accuracy, macro precision and macro recall for the classifier.
You may or may not use the scikit-learn implementations for computing these metrics.

k-fold Cross
K-fold cross-validation is a technique used to assess and optimize the performance of machine
learning models. The dataset is divided into K subsets, or ”folds.” The model is trained on K-1 folds
and tested on the remaining one. This process is repeated K times, and the average performance
is used to gauge the model’s generalization ability.
For this assignment,
1. Split the dataset into 80% for training and 20% for testing. Normalize/Regularize data if
necessary. Encode categorical variables using appropriate encoding method if necessary.
2. Train a Logistic Regression model on the dataset using saga solver from scikit-learn
package and using no regularization penalty.
3. Cross Validate the classifier with 5-folds and print the mean accuracy, precision and
recall for the class 1(good) for the classifier. You may or may not use the scikit-learn
implementations for computing these metrics. However, you cannot use any ML package
for the cross validation logic.
