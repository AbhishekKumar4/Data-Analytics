# Bar Graphs Using Python

Code for plotting bar graph : 

````
import pandas as pd
import matplotlib.pyplot as plt



dataset = pd.read_csv('Abduction_Data.csv')

dataset.drop('Crime head',axis = 1, inplace = True)

#Get all states
x = dataset.iloc[:, 0].values
#Get all crimes
y = dataset.iloc[:, -1].values

plt.xticks(rotation = '90')
plt.title('Crime Statistics')
plt.xlabel('Countires')
plt.ylabel('Total Crimes Recorded')

plt.bar(x, y)
plt.show(block=True)
````

![alt text](https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Descriptive%20Statistics%20-%20%20Graphical%20Approaches/2.%20For%20Qualitative%20Categrical%20Variables/Bar%20Graphs/Bar%20graphs%20using%20python/Crims_Stats.PNG)

Make it more interesting bu just adding below line

````
import matplotlib.cm as cm
import numpy as np
plt.bar(x, y)
plt.bar(x, y, color = cm.rainbow(np.linspace(0, 1, len(x)))) //added line
plt.show(block=True)


````

![alt text]()
