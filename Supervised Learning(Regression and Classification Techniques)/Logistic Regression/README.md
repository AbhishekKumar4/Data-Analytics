# Logistic Regression

**Problem Statement**

- We have looked at the problems of classification earlier and here is the example of earlier model.

![alt text]()

- Goal of classification is to find the decision surface that will helkp us separate people who buy the computer from those who do not.
- Let us take a step back and ask what exactly does this decision surface means? or what is a data point that lie on the decision surface belong to is it buy computer or does not buy computer.
- One way of thinking about it is to say that this decision surface denotes all the data points for the probability of it being red = probability of it being brown. i.e P(red|x) = P(brown|x)

![alt text]()

it mean for the points on the decision surface we are not able to make decision weather it will buy or not.

- And does it tell us about the points that lies on one side of the boundry(decision surface) i.e probability of person not buying computer > buying --> P(Red|x) > P(Brown|x)

- One way of thinking abot the decision boundry is that it models all the points where both the classes are equally likely or equaly probable to occur.

**Going beyond classification**

- Interested in knowing the actual probability of a specific class given a data point not just finding the right classification. example : medical domain, suppose patient has a specific disease, we would like to know that how confident is the doctor of the prediction and doctor says that he is 90% sure that he has this disease. so its better to go for treatment.
- So likewise when you have a classifier that is going to give you a class label. we would like to know that how sure the classifier of the class label and thats one application where we would like to see these kinds of probabilities.
- One way to approach predicting probabilities instead just of the class lables could be to treat it as a regression problem.

# classification as a regression problem or Pregression of classification**

- We have labels (example : persons who buys computer and persons who dont).
- Instead of using this label we can use indicator variables for the classes example : person who buys computer --> 1, and who doesnot --> 0.
- Now our data is transformed into a regression problem instead of classification.

X1 = (30,000, 25), Y1 = Doesnot buy

X2 = (80,000, 45), Y2 = Buys computer

transformed to,

X1 = (0.15, 0.25), Y1 = 0

X2 = (0.4, 0.45), Y2 = +1

- Now use linear regression.
- F(x) can be interpreted as P(Y = 1/X)

**Problems with this approach**

- Linear regression is not limites in range, output can go from -infinity to +infinity therefore can not be interpreted in probability.
- Output can not be interpreted as a probability as it can be negative.
- Works in practice but not that well.

**Solution is Linear Regression**

- We can still use linear regression on a transformed function.
- Logistic or logit function.
 - Log odds.
 - Let p(x) denote the p(y=1|x) than logit transformation is given by:
   
   ![alt text](https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Supervised%20Learning(Regression%20and%20Classification%20Techniques)/Logistic%20Regression/logit_transformation.PNG)
   
- So in short we are takin g a ration of probability o success to probability of failure known as log-odds function. 
 
 







