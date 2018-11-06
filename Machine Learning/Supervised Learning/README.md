# Supervised Learning

The majority of practical machine learning uses supervised learning.

Supervised learning is where you have input variables (x) and an output variable (Y) and you use an algorithm to learn the mapping function from the input to the output.

Y = f(X)

The goal is to approximate the mapping function so well that when you have new input data (x) that you can predict the output variables (Y) for that data.

It is called supervised learning because the process of an algorithm learning from the training dataset can be thought of as a teacher supervising the learning process. We know the correct answers, the algorithm iteratively makes predictions on the training data and is corrected by the teacher. Learning stops when the algorithm achieves an acceptable level of performance.

Supervised learning problems can be further grouped into regression and classification problems.

**Classification:** A classification problem is when the output variable is a category, such as “red” or “blue” or “disease” and “no disease”.

**Regression:** A regression problem is when the output variable is a real value, such as “dollars” or “weight”.
Some common types of problems built on top of classification and regression include recommendation and time series prediction respectively.

Some popular examples of supervised machine learning algorithms are:

- Linear regression for regression problems.
- Random forest for classification and regression problems.
- Support vector machines for classification problems.

# Classification

Suppose we are given some data of age and income of customer coming to buy a laptop plotted with customer who bought the laptop and who doesn't.

- Simplest model would be to draw a straight line. i.e people who are below certain income are not going to buy laptop and people above certain incoe are going to buy the laptop.
- We have to be really cautious that we do not end up modelling noise in data that leads us to make wrong predictions in future data.

![alt text]( https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Machine%20Learning/Supervised%20Learning/supervised-learning-classification.png)

# Inductive Bias/Inductive Learning

- Our goal is just not to do well on the training data. If we are only interested in doing well in training data the best way to do it then is just to remember all the data points given to us so that we dont make mnistakes again.
- Our goal is to perform well on the data that we have never seen before. We need to generalize on unseen data and the only way to generalize on unseen data is by mainly assumptions about the model.
- **Need to generalize assumptions about the line**
- Such assumptions on models that we are generating are called as Inductive Bias.

**Inductive bias is of two types**

**Language Bias**
Is essentially the restrictions that we had on the kind of line i.e If we say, we are nly going to consider straight lines that are parallel to x-axiz or y-axis, its one kind of language bias.

**Search Bias**
Given that we have already selected the language in which we are going to represent our classifier. How do we search among the possible classifiers in that language in order to find the right one.

# Supervised Learning Process

![alt text]( https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Machine%20Learning/Supervised%20Learning/SupervisedProcess.png)

# Training

![alt text]( https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Machine%20Learning/Supervised%20Learning/Training_SL.png)

# Applications of classification

- Credit card fraud detection
  - Valid transaction or not.
- Sentiment Analysis/Opinion mining/Buzz Analysis
  - On social media or any other paltform weather someone is saying positive or negative about subject.
- Churn Prediction (potential churner or not)
  - User of sevice likely to leave soon. for example switching from vodafone to airtel or vice versa, take measure to retain them.
- Medical diagnosis and also in risk analysis.
