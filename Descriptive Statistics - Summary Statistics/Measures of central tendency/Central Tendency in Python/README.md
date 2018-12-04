# Measures of Central Tendency in Python


  ````
import pandas as pd
import numpy as np
from scipy import stats

dataset = pd.read_csv('UP_Crime_stats.csv')

#Get all crimes
crimes = dataset.iloc[:, -1].values
print(crimes)
crimes = sorted(crimes)
print(crimes)
mean_value = np.mean(crimes)
print('Mean Value : ', mean_value)

median_values = np.median(crimes)
print('Median Value : ', median_values)

range = np.ptp(crimes)
print('Range : ', range)

variance = np.var(crimes)
print('Variance : ', variance)

std_deviation = np.std(crimes)
print('Standard Deviation : ', std_deviation)

standard_error = stats.sem(crimes)
print('Standard Error : ', standard_error)
  
  ````
  
  **Add code to plot a histogram**
  
  ````
plt.hist(crimes,bins=10,color='grey')
plt.axvline(mean_value,color='red',label='Mean')
plt.axvline(median_values,color='yellow',label='Median')
plt.xlabel('Crimes')
plt.ylabel('Frequency')
plt.legend()
plt.show()
  
  ````
