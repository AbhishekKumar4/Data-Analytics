# Two Sample Tests

What is the difference?
- Here we will get two sets of data.
- To make some statement about mean/proportions/variance of population 1 and population 2.
- Single set of data v/s two sets of data.
Think of it a dealing with two variables for the first time.

Examples : 

 - Changing the tempreture in a manufacturing process to see if the mean number of defects decreases. In this example our first variable is temprature and second variable is number of defects.
 - Two different manufacturing processes to compare variance of finished products in each batch. In this case our first variable is manufacturing process and second variable is variance (diameters) of products.
 - Are 10th standard girls taller than 10th standard boys in india. In this case, first variable is gender and second variable is height.
 
 # Test
 
 Almost the same as single sample hypothesis testing with some adjustments.
 
  - Have a null and alternate hypothesis. Ho = u1 = u2 and H(alt) : u1 =/(not equal) u2.
  - Calculate the test statistic.
  
  
  
  Here (u1-u2) is degrees of freedom (DOF). if u1 = u2 than DOF=0 and if mean is 3 units higher. i.e u1 = u2 + 3 than DOF=3.
  - This is the Z-Distrubution or N(0,1sq).
  - Use Z tables, excel, R or matlab.
  - Low enough p value is grounds for rejecting the null hypothesis.
 
