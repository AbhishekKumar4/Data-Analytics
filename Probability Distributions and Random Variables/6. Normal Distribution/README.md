# Normal Distribution

- The normal distribution is the most important probability distribution in statistics because it fits many natural phenomena.
- It is also known as the Gaussian distribution.
- Sometimes called the bell curve,  is a distribution that occurs naturally in many situations.
- The bell curve is symmetrical. Half of the data will fall to the left of the mean; half will fall to the right.

# Properties of a normal distribution
The mean, mode and median are all equal.The curve is symmetric at the center (i.e. around the mean, μ). Exactly half of the values are to the left of center and exactly half the values are to the right. The total area under the curve is 1.

**PMF is given by,**

![alt text]( https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Probability%20Distributions%20and%20Random%20Variables/6.%20Normal%20Distribution/normal_distribution.png)

However, **CDF is not something that simplifies very elegantly.** So, to define the CDF you would still use your traditional procedure of using the integral and by the way the normal distribution goes from minus infinity to plus infinity

**So, the CDF is often just stored in tables, sometimes especially for the normal with mean 0, standard deviation 1 or it is just something that we integrate each time to get.**

Unlike the uniform distribution, which says everything is equally likely. It is the normal distribution says that things in the extremes are less likely, things in the center are more likely within certain limits, which is what gives it its characteristics bell shaped curve. There are many other distributions also like this, many things after you remove outliers start to look normal.

# Binomial Approximation or normal approximation of the binomial distribution.

Although, the binomial is a discrete distribution and the normal is a continuous distribution. The normal distribution can be used as an approximation to the binomial distribution
I
- When n becomes really large we can essentially use this formula that we have for mean and variance of the binomial distribution and construct a normal distribution, with this mean and variance we can answer distribution related questions.
- In some cases, working out a problem using the Normal distribution may be easier than using a Binomial.
