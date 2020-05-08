#### Exercise 1

Our goal is to predict whether a wildfire will reach the wildlife protection zone, as denoted by the indicator variable `wlf`. Previously we utilized boosting, bagging, and random forests methods to build candidate models. We also benchmarked those methods against a logistic regression model that utilized all predictors. In this lab, you will use a support vector classifier and support vector machines.

A. Tune a support vector classifier with a linear kernel to select an optimal `cost`. Consider values in the range 0.01 to 10. Compute the training and test error rates using this new value for cost. (**Hint:** You can use the `tune()` function or `crossv_kfold()` to tune your model.)

B. Tune a support vector classifier with a radial kernel to select an optimal `cost`. Use the default value for `gamma` and try to determine your own range of values for `cost` to explore.

C. Tune a support vector classifier with a polynomial kernel to select an optimal `cost`. Use the default value for `degree` and try to determine your own range of values for `cost` to explore. 

D. Calculate the test error for each of the 3 candidate classifiers selected in parts (A) - (C). Which classifier is the best? 

E. Construct a table displaying the test error for these 3 candidate classifiers, the candidate models from L02 CART, and the multiple logistic regression fit in L02 CART.
<br><br>


### Challenge 1 (Not Mandatory)

Use the `ggroc()` function from the `pROC` package to construct ROC curves for the SVM candidate classifiers from above. Do this for each classifier on both the training and testing sets.    
<br><br>


### Challenge 2 (Not Mandatory)

Expand your solution to **Exercise 2(B)** where you fit a radial kernel SVM, and tune your model to find an optimal value of `gamma`. You can either tune `gamma` fixing the `cost` to the optimal value you found in Exercise 2(B). Alternatively, you can jointly tune both `gamma` and `cost`.
<br><br>


### Challenge 3 (Not Mandatory)

Expand your solution to **Exercise 2(C)** where you fit a polynomial kernel SVM, and tune your model to find an optimal value of `degree`. You can either tune `degree` fixing the `cost` to the optimal value you found in Exercise 2(B). Alternatively, you can jointly tune both `degree` and `cost`.
<br><br>
