# Scatter Plot In Python

**Code**

````
import pandas as pd
import matplotlib.pyplot as plt
import numpy as np


dataset = pd.read_csv('UP_Crime_stats.csv')

#dataset.drop('Crime head',axis = 1, inplace = True)

#Get all years
year = dataset.iloc[:, 0].values
#Get all crimes
crimes = dataset.iloc[:, -1].values

colors = (0, 0, 0)
area = np.pi * 3

# Plot
plt.scatter(year, crimes, s=area, c=colors, alpha=0.5)
plt.title('Scatter plot in python')
plt.xlabel('Year')
plt.ylabel('Crimes')
plt.show()


````


**Output Image**

![alt text](https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Descriptive%20Statistics%20-%20%20Graphical%20Approaches/3.%20For%20Multiple%20Variables/Scatter%20Plots/Scatter%20plots%20in%20python/sc_plot_in_python.PNG)
