# Data and Algorithmic Modelling

# K Nearest neighbours techniques

- New supervised learning approach.
- By introducing this technique and comparing it to something we already know which is regression analysis.
- By doing this comparision we are hoping to illustrate or appreciate two very different styles of performing a supervised learning analysis and process of prediction itself.
- By this we learn that there are lots of other techniques too which takes inspiration from this approach.
- Breimen L (2001) said that statistical modelling is of two styles or two cultures.

# 1. Data Modelling Approach

- For example standard regression.
- Where we have some output variable Y and we envision this output variable as some function of our input.

Example: for linear regression Y = f(x) + E(Noise), for multiple regression and also with discriminant analysis etc.

- Alll captures functional relationships between y and x and that function is in some sense cast in stone and the only job we are left with is to go get the data and figure out what the parameters are of the function.

# 2. Algorithmic Modelling Approach

- Focus is not much on rigid mathematical model that we have pre supposed, which creates a relationship between x and y.
- But instead we really have a set of algorithmic instructions or algorithmic ideas that relate the independent and dependent variable.
- In loose sense y is function of x but that is captured by algorithms rather than rigi mathematical models.

Example: K nearest neighbours and random forests etc.

# Prediction

- Goal is to understand KNN approach.
- Lets discuss how prediction task happens with linear regression approach.

**The Regression Approach**

The way it happens is:

- We have some data.
- We do regression analysis(it fits a line through the data).
- Its a line that minimizes the squared deviation(if we are doing ordinary least squares).
- and we make prediction.
- Than someone asks what Y we can expect given this X.
- So we draw a line from x1 and see what value of Y we are getting based on our fitted model.
- After this we dont need this data points, we can erase them.
- Alll we need to know is the line we created with regression.

