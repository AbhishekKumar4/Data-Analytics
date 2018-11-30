# Bar Graphs Using Python


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
