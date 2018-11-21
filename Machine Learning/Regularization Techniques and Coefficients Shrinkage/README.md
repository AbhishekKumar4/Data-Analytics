# Regularization Techniques and Coefficients Shrinkage

- How do we go about choosing our input variable? The problem of subset selection.
- Huge overlap with subset selection.
- Adjusted R(square) and coefficient shrinkage in continuation to subset selection in multiple regression.
- How do we measure, how good the model is?
- How to get good predictive accuracy, and its also useful for interpretation.
- Core idea being, how can we simplify our model in some sense because we care about predictive accuracy and interpretation. We dont care about just trying to get this function to go through all of our data points.


**Metric to evaluate a regression model**
- So far we have discussed the p-value from the f-test of an ANOVA.
- Can we use this p-value as a guide to see which varibales stays and which variables stays out. For doing this apart from measures like forwards,backwards and hybrid etc we have two more methods called R(square) and adjusted R(square).

**R(square) and adjusted R(square)**
- R(square) is not a very good measure in terms of how the overall regression model is specially in a multiple regression context.
- R(square) is a measure of how much of our variation is in terms of Y(output variable). So, how much of our output variation and how much of that we can explain using our model and how much is that we can not explain using our model. So, we take the overall variation of Y and break it into two chunks. The amount that can be explained by our model, which is our regression equation. and the amount that can not be explained by that. If we put thosetwo together, we should get the overall variation in Y irrespective of X.
- **So, R(square) is nothing but this ration of how much variation is explained by the model divided by total variation.**
- Total variation is also known as sum of squares total i.e **SST**.
- Sum of squares model variation(SSM) / sum of squares regression

R(square) = SSM / SST

- So from ANOVA test we have only one equation left i.e SSE(sum of squares error) also known as residual sum of squares(RSS).

- Total squared distance of each data point from the grand mean.

![alt text](https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Machine%20Learning/Regularization%20Techniques%20and%20Coefficients%20Shrinkage/SST.PNG)

- Each predicted value and look at deviation from grand mean.

![alt text](https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Machine%20Learning/Regularization%20Techniques%20and%20Coefficients%20Shrinkage/SSM.PNG)

- How much is each data point is deviating from each predicted value.

![alt text](https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Machine%20Learning/Regularization%20Techniques%20and%20Coefficients%20Shrinkage/SSE.PNG)


R(square) is not so good as discussed because, R(square) by defination will only increase as we keep on adding more and more variables.(Later to be discussed in Bias-Variance Dichotomy)

**Therefore another metric that we can use is Adjusted R(square)**
 
 - Modified version of R(square).
 
 ![alt text](https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Machine%20Learning/Regularization%20Techniques%20and%20Coefficients%20Shrinkage/AdjustedRsquare.PNG)
 
 - Goal is for higher R(square) but K as minimum.
 
 
 *Continuation of Regularization Techniques and Coefficients Shrinkage*
 
Suppose we have an algorithm and we have fixed number of input variables. So, we are no longer bargaining to throw away variables out or keep them in. But is there some way in our fitting methodology itself, preventing this problem of over-fitting, preventing to get the functional form to be so hard wired to the data that it does not do a good job of predicting and kind of imposing penalties upon ourselves to kind of overfitting.
 
- One way in which overfitting happens is problem of multi-colinearity(idea that many of input variables are co-related with each other).
 - Ex : Y = 4A - 2B, imagine if A and B are co-related to a point where they are practically same variable than a fitted model i.e Y = 10A - 8B should also kind of give us the same results in a sense that A and B are practically same data points.
 - In cases like this we want to have the simplest possible equation and lowest possible magnitudes for variables.
 
 Y = 2A - 0B, here 2 is magnitude. How can we achieve this?(In next point)
 
 - In really siple terms not just allowing highly co-related variables to take up opposing sides and have really large co-efficients(By using standard least squares minimization).
 
 
# Ridge Regression

![alt text](https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Machine%20Learning/Regularization%20Techniques%20and%20Coefficients%20Shrinkage/RRminization.png)


# Lasso Regression
- Almost same , just the subject to constaint is different.

![alt text](https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Machine%20Learning/Regularization%20Techniques%20and%20Coefficients%20Shrinkage/lassoR.png)
 
 
 
 

