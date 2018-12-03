# Pie Charts Using Python


Code chunk for drawing pie chart : 

````
import pandas as pd
import matplotlib.pyplot as plt
import matplotlib.cm as cm
import numpy as np


dataset = pd.read_csv('Abduction_Data.csv')

dataset.drop('Crime head',axis = 1, inplace = True)

#Get all states
x = dataset.iloc[:, 0].values
#Get all crimes
y = dataset.iloc[:, -1].values

plt.pie(y, labels=x, startangle=90, autopct='%1.1f%%')
plt.title('Total Crimes Recorded')
plt.show()

````

![alt text](https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Descriptive%20Statistics%20-%20%20Graphical%20Approaches/2.%20For%20Qualitative%20Categrical%20Variables/Pie%20Charts/pie%20charts%20using%20python/pie_Chart.PNG)

