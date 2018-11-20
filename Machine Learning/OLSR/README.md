# Ordinary Least Squares Regression

- Regression is supervised learning tool.
- Ordinary least squares (OLS) regression is a statistical method of analysis that estimates the relationship between one or more independent variables and a dependent variable.
- The method estimates the relationship by minimizing the sum of the squares in the difference between the observed and predicted values of the dependent variable configured as a straight line. 
- At a very basic level, the relationship between a continuous response variable (Y) and a continuous explanatory variable (X) may be represented using a line of best-fit, where Y is predicted, at least to some extent, by X.
- If this relationship is linear, it may be appropriately represented mathematically using the straight line equation 'Y = mx +c' or 
  'Y = b0 + b1x'
- Concept of actual Y(Yi) and estimated Y(Yi)
- Looks like there is this value of Y1 and it corresponds to some x1 and we are going to take x2 and see where our line goes through in terms of Y values.
- We are trying to minimize the squared deviation between the actual and estimate.
- Summation (Y1actual - Y1estimate)square --> How close the line is to its data points.

**What we are trying to do in** ordinary least square regression is to figure out that line, and how do we define a line? we define it by Bo and B1, once we fix that B0 and B1 the line gets fixed. So we are going to try and figure out that B0 and B1 which defines the line, which results in minimizing the squared deviation between actual and estimate.

Because there may be another line with another B0 abd B1 which is very far away from the data points, so the squared deviations are going to be huge
