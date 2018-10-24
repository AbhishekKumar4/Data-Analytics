# Uniform Distribution

**The uniform distribution has a discrete version and a continuous version**

# Discrete uniform distribution

Uniform distribution, sometimes also known as a rectangular distribution, is a distribution that has constant probability.

![alt text]( https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Probability%20Distributions%20and%20Random%20Variables/1.%20Uniform%20Distribution/uniform.png)

For instance we have a six sided dice, and we are quantifying the probability of getting any particular face values. So, the face value of the dice is essentially, we throw the dice and get something on top, so you see the 1 or 2 or 3 or 4 or 5 or 6. So, the probabilities associated with these 6 possible outcomes, assuming a fair dice is one sixth for each and, so that is example of discrete uniform distribution. 
We also have the case of the coin toss, where we only have two possible outcomes and as long as they are both equal, it is still uniform.

**The formula in terms of the PDF the Probability Density Function, is just 1/k when there are k outcomes.**
So, if this is 6 sided dice it is 1 by 6 for each of those six possible outcomes. If it is coin toss, which is two possible outcomes it is going to be 1 by 2 and the ideas that for each of those k possibilities, it is 1 by k and for the rest of the universe, it is 0.

# Real world example
There are not a lot of examples, real world things that tend to be uniforms.
- Some of them are something like number of seconds pass the minute. So, if we were to randomly, if we have a random process. we just looked at the clock over the course of date during some random intervals, the number of the seconds pass the last minute could be uniform and that is essentially a space, where we can have 0 seconds pass the minute all the way to 60 seconds pass the minute. So, our interval is from 0 to 60 and where we find ourself in that interval is described potentially by uniform distribution. And again the idea that it is continuous, just means that you not discretized the seconds as 1 or 2 or 3 all the way to 60, you could be in that in 4.5432 seconds pass the minute. So, it is continuous, the variable time is being monitored continuous as a continuous variable.

- Another example could be the exact age of the randomly selected person between the ages of 50 and 60 in a certain country. Now, again we know we have to come up with fairly specific examples, because something simple like the age of the randomly selected person is not likely to be uniform. we are not likely to find as many people between 80 and 90, as we are between 70 and 80.

But, sometimesover a short enough interval, even if the overall distribution is not uniform we can create an interval and say that is our universe. our universe is people between the age 30 to 40, within that interval perhaps the distribution of the exact age of people. So, imagine we take the universe of all people between the ages of 30 to 40 in India and then, try to create a distribution of the exact age of a randomly selected person from this bucket and that could potentially be a uniform. The uniform is also a great distribution, think of when we want to make absolutely no assumptions.

The uniform distribution can be thought of like ground 0, we do not make any assumptions, the probability of everything occurring within a certain interval is equal and we can potentially use it.

**For continuous uniform distribution PDF is essentially 1 by b minus a.**

**CDF of this distribution? Again, it is x minus a by b minus a.**

![alt text](https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Probability%20Distributions%20and%20Random%20Variables/1.%20Uniform%20Distribution/PDF%26CDF.png)
