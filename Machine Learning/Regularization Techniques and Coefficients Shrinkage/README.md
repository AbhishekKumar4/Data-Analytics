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

- So from ANOVA test we have only one equation left i.e SSE(sum of squares error) also known as residualsum of squares(RSS).

- Total squared distance of each data point from the grand mean.

![alt text]()

- Each predicted value and look at deviation from grand mean.

![alt text]()

- How much is each data point is deviating from each predicted value.

![alt text]()

