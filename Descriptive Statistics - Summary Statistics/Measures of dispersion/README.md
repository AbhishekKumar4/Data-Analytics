# Measures of Dispersion

As now we know how measures of central tendency try to captures, what appears to be like a central value. Measures of dispersion talk really about, how the data is dispersed around this central value, how does the data deviate from this central value.

For instance, for now assume that 10 is our measure of central tendency. One measure of central tendency is the mean, let us just say we are using the mean. So, 10 is the mean, then if every single data point in this data set was equal to 10. Then, there would be no deviation of data from 10. Typically, most data sets, the values are going to be different and we might have some measure of central tendency, but there is going to be some amount of deviation of the data points on either side to the central value. Now, measures of dispersion try to capture that, do the values deviate a lot from the center or do they deviate very little from this center and that is what measures of dispersion seek to capture.

# Different measures of dispersion

1. **Range** : The simplest measure of dispersion is range and the range is quite simply nothing but, the highest value minus the lowest value of our data set.

For example : Data set : 3, 4, 3, 1, 2, 3, 9, 5, 6, 7, 4, 8
Range would be : Max - Min (9 - 1) = 8

Given that the mean of this data set is about 4.5, 4.6, a measure of dispersion is just the max minus min. Now, if for instance if there was very low dispersion, then the highest value would be close to 4.6 and the lowest value would be close to 4.6 and so that, range between max minus min could have been smaller. At the same time, if this dispersion is very high, on the high side and on the low side of our max and min value is going to deviate a lot from the 4.6 and so, we would have high dispersion.

2. **Inter Quartile Range** : The idea here is highly related to the concept of median, where we would arrange the data points and we would kind of take a central data point. we discussed that procedure of median during measures of central tendency, but another way of thinking of it is that, we are taking the 50th percentile point. With the Inter Quartile Range, what we are doing is we are taking the 75th percentile point or the 3rd quartile and subtracting from at the 25th percentile point.

The idea being that within this data set if there is a high level of dispersion, then that range between the 75th percentile point to the 25th percentile point also be high and if the dispersion is low, then this range would be low and it is really noteworthy that this is the concept that gets captured in **box plots** , which we discussed in a graphical techniques. We spoke about, how in the box plots the upper line of the box plot and the lower line of the box plot, correspond usually to the third quartile and the first quartile of our data set. So, and this is also known as the Inter Quartile Range. So, it might be abbreviated to IQR in some text books, but this is also a measure of dispersion.

3. **Standard Deviation** : The Standard Deviation is also a measure of how spread out numbers are. Its symbol is σ (the greek letter sigma).
The formula is easy: it is the square root of the Variance. So now you ask, "What is the Variance?"

**Variance** : The average of the squared differences from the Mean.To calculate the variance follow these steps:
(a) Work out the Mean (the simple average of the numbers)
(b) Then for each number: subtract the Mean and square the result (the squared difference).
(c) Then work out the average of those squared differences. (Why Square?)

**(Why Square?)** If we just add up the differences from the mean ... the negatives cancel the positives

If we just add up the differences from the mean ... the negatives cancel the positives:

![alt text]( https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Descriptive%20Statistics%20-%20Summary%20Statistics/Measures%20of%20dispersion/sd1.gif)  4 + 4 − 4 − 44  = 0
So that won't work.

![alt text]( https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Descriptive%20Statistics%20-%20Summary%20Statistics/Measures%20of%20dispersion/sd1.gif)  |4| + |4| + |−4| + |−4|4  =  4 + 4 + 4 + 44 = 4
That looks good, but what about this case:

![alt text]( https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Descriptive%20Statistics%20-%20Summary%20Statistics/Measures%20of%20dispersion/sd2.gif)  |7| + |1| + |−6| + |−2|4  =  7 + 1 + 6 + 24 = 4
Oh No! It also gives a value of 4, Even though the differences are more spread out.

So let us try squaring each difference (and taking the square root at the end):

![alt text]( https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Descriptive%20Statistics%20-%20Summary%20Statistics/Measures%20of%20dispersion/sd1.gif)  √( 42 + 42 + 42 + 424 ) = √( 644) = 4

![alt text]( https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Descriptive%20Statistics%20-%20Summary%20Statistics/Measures%20of%20dispersion/sd2.gif)  √( 72 + 12 + 62 + 224 ) = √( 904) = 4.74...
That is nice! The Standard Deviation is bigger when the differences are more spread out ... just what we want.

**But ... there is a small change with Sample Data**
If the data is a Sample (a selection taken from a bigger Population), then the calculation changes!

When you have "N" data values that are:

The Population: divide by N when calculating Variance.
A Sample: divide by N-1 when calculating Variance.


**Formulas**
Here are the two formulas for Standard Deviation Formulas if you want to know more:

    The "Population Standard Deviation":

 	![alt text]( https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Descriptive%20Statistics%20-%20Summary%20Statistics/Measures%20of%20dispersion/formula1.gif)

	The "Sample Standard Deviation":	 	
	
	![alt text]( https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Descriptive%20Statistics%20-%20Summary%20Statistics/Measures%20of%20dispersion/formula.png)