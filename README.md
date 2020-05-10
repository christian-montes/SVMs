#### Exercise 1

Our goal is to predict whether a wildfire will reach the wildlife protection zone, as denoted by the indicator variable `wlf`. Previously we utilized boosting, bagging, and random forests methods to build candidate models. We also benchmarked those methods against a logistic regression model that utilized all predictors. In this lab, you will use a support vector classifier and support vector machines.

A. Tune a support vector classifier with a linear kernel to select an optimal `cost`. Consider values in the range 0.01 to 10. Compute the training and test error rates using this new value for cost. (**Hint:** You can use the `tune()` function or `crossv_kfold()` to tune your model.)

B. Tune a support vector classifier with a radial kernel to select an optimal `cost`. Use the default value for `gamma` and try to determine your own range of values for `cost` to explore.

C. Tune a support vector classifier with a polynomial kernel to select an optimal `cost`. Use the default value for `degree` and try to determine your own range of values for `cost` to explore. 

D. Calculate the test error for each of the 3 candidate classifiers selected in parts (A) - (C). Which classifier is the best?