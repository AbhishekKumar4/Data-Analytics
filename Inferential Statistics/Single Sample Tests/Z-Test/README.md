# Z-Test

Single sample z-test is a test that is used when we want to make some inferences about the population mean. Note that we are saying using the sample, but we are not interested in just reporting the sample mean, which is what we might we done with descriptive statistics; but, we are interested in ultimately making a statement about the population means. And, this is a test, where we need to know the variance or standard deviation.

**What are we testing?**
Population mean. We have a sample but with this sample we want to say something about the population mean.

**Useful when we know the standard deviation or variance.**

**When sample size is very large i.e >=30. When sample size is >=30 we have large enough sample that we can actually calculate the variance from the data and use it.**

Example: Average phosphate level in blood is <=4.8 mg/dl, with a known standard deviation of 0.4 mg/dl.
Data : 4.1, 3.9. 5.3, 4.7 ........

Now we have sample data, we need to say something about the population.

Step 1: Check null hypothesis.

Step 2: Calculate the 'test statistics'.

![alt text]( https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Inferential%20Statistics/Single%20Sample%20Tests/Z-Test/zscoreformula.png)

Step 3: If the null hypothesis is true, than the z-statistic should be the same or equivalent to pulling a random number from a z-distribution or N(0, 1), with mean 0 and variance 1. The z-distribution is nothing but a normaldistribution with mean of 0.

Step 4:  Check if z-stat actually look like it could be something that we could havepulled out of a N(0,1 square), because if it does not, then something that we assumed was wrong.

Step 5:  Ff it turns out that the z-stat is too extreme a value to be coming from this normal distribution, then we can maybe make
a statement about the null hypothesis.

Step 6: Calculate p-value, it is the probability of seeing a test statistic as extreme as the calculated value if the null hypothesis is true. If it looks too extreme, and the p value of the probability of seeing this test statistic is really low; then, perhaps the null hypothesis was not true to start with.

For instance out here, if the z-statistic you computed was 1.2. I am going to compute a probability; and, this – the probability is a probability to
the right side of 1.2. It is the area under the curve out here. And the idea is because We are then quantifying the probability of seeing something as extreme as 1.2 or greater than is equal to the area under this curve. That might happen to be any value. So, if it happens to be something like 13 percent or whatever. But, if this number was really low; if this number was 0.001. The standard thing that you do is you fail to reject the null hypothesis; you technically never accept the null hypothesis.


In most of the scenarios people work with two-tailed case. two tailed case, where your null hypothesis is really that for example mu is equal to 4.8. And, we are interested in rejecting this null hypothesis whether that mu is too large; meaning it is large enough that we can say that it cannot be equal to 4.8; or, if it is small enough. So, we are happy to reject if we see evidence that shows that mu cannot be 4.8 on either account; maybe because it is the data suggests that it is too large, maybe because the data suggests that it is too small. And, that is called the two-tailed case.




