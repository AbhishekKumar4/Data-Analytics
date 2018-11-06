# Regression or Prediction (Predicting a continuous value)
Regression predicts a continuous target variable Y. It allows you to estimate a value, such as housing prices or human lifespan, based on input data X.

Here, target variable means the unknown variable we care about predicting, and continuous means there aren’t gaps (discontinuities) in the value that Y can take on. A person’s weight and height are continuous values. Discrete variables, on the other hand, can only take on a finite number of values — for example, the number of kids somebody has is a discrete variable.

**Try to minimize the sum of squared error while prediction.**
Figure out the difference between the line, the prediction made by the line that we fit and the actual data point that was recorded and take the square of the error and try to minimize that.

# Linear Regression
- “Draw the line. Yes, this counts as machine learning.”
- Minimize the sum squared error.
- With sufficient data, simple enough is just to set matrix operations.
- With many dimensions, challenge is to avoid overfitting and this can be avoided by adopting **Regularization**(Ensure that of all the models that can fit the data to a certain extent, we will try to find something which is simple enough so that we do not overfit the data)
- Higher order functions. How do we handle them? We handle them by **Basis Transformation**. For example : We take the input x1 and x2 and than we translate it to a much larger description by adding second order terms.

(x1, x2) -->  {x1(square). x2(square), x1x2, x1, x2}

# Applications Of Regression

- Time series prediction
  - Rainfall in a certain region.
  - Expenses on voice calls.
- Classification
  - What is the probability that the person is going to buy laptop.
- Data Reduction
  - Instead of giving 10,000 points we can give low dimentional line/curve to that and simply tell the parameters of the line.
- Trend Analysis
  - More interested in the data analysis than prediction. we would like to know weather the growth rate is linear or exponential.
- Risk factor analysis
  - Factor contributing most to the output. example : In linear regression, the input variable which has larger cofficient is the one who is going to be influencing the output most.
