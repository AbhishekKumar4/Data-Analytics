# Setup

- This guideline is to get us starting with python.
- This includes installing pip package manager for python.
- Installation of libraries needed for data processing in python.

**Installing pip for python**

- Make sure that we have included python home in path variable of system, this will enable us to use intall pip using command.
- Download pip package from [pip](https://pip.pypa.io/en/stable/installing/)
- Go to the directory in which you have downloaded pip package.
- Execute command python get-pip.py

**You may get this error message**

```
Collecting pip
  Retrying (Retry(total=4, connect=None, read=None, redirect=None, status=None)) after connection broken by 'ConnectTimeoutError(<pip._vendor.urllib3.connection.VerifiedHTTPSConnection object at 0x0000027E81D656D8>, 'Connection to pypi.org timed out. (connect timeout=15)')': /simple/pip/
  Retrying (Retry(total=3, connect=None, read=None, redirect=None, status=None)) after connection broken by 'ConnectTimeoutError(<pip._vendor.urllib3.connection.VerifiedHTTPSConnection object at 0x0000027E81D65D30>, 'Connection to pypi.org timed out. (connect timeout=15)')': /simple/pip/
  Retrying (Retry(total=2, connect=None, read=None, redirect=None, status=None)) after connection broken by 'ConnectTimeoutError(<pip._vendor.urllib3.connection.VerifiedHTTPSConnection object at 0x0000027E81D65FD0>, 'Connection to pypi.org timed out. (connect timeout=15)')': /simple/pip/
  Retrying (Retry(total=1, connect=None, read=None, redirect=None, status=None)) after connection broken by 'ConnectTimeoutError(<pip._vendor.urllib3.connection.VerifiedHTTPSConnection object at 0x0000027E81D8D160>, 'Connection to pypi.org timed out. (connect timeout=15)')': /simple/pip/
  Retrying (Retry(total=0, connect=None, read=None, redirect=None, status=None)) after connection broken by 'ConnectTimeoutError(<pip._vendor.urllib3.connection.VerifiedHTTPSConnection object at 0x0000027E81D652B0>, 'Connection to pypi.org timed out. (connect timeout=15)')': /simple/pip/
  Could not find a version that satisfies the requirement pip (from versions: )
No matching distribution found for pip

```

In this case try adding proxy : 

````
D:\>python get-pip.py --proxy="http://url"
````

- Install required libraries

````
python -m pip install --user numpy pandas --proxy="url"
````
# Data PreProcessing

**1. Importing libraries and dataset**

````
import pandas as py
dataset = py.read_csv('Customers.csv')
# select all the rows and all columns except the last column
X = dataset.iloc[ : , :-1].values

# select all the rows data from 3rd column
Y = dataset.iloc[ : , 3].values

````
if we print X and Y, we get below results

````
print(X)
[['France' 44.0 72000.0]
 ['Spain' 27.0 48000.0]
 ['Germany' 30.0 54000.0]
 ['Spain' 38.0 61000.0]
 ['Germany' 40.0 nan]
 ['France' 35.0 58000.0]
 ['Spain' nan 52000.0]
 ['France' 48.0 79000.0]
 ['Germany' 50.0 83000.0]
 ['France' 37.0 67000.0]]
 
print(Y)
['No' 'Yes' 'No' 'No' 'Yes' 'Yes' 'No' 'Yes' 'No' 'Yes']

````
**2. Handling missing values**
 - Data can be missing due to various reasons.
 - Handle missing data so it does not impact the performance of machine learning model.
 - Missing values can be replaced by mean, median or mode of entire column
 - Can use Imputer class from sklearn.preprocessing
 - Getting warning as imputer is marked as deprecated.
 - SimpleImputer can be used in place of Imputer.

````
from sklearn.preprocessing import Imputer
imputer = Imputer(missing_values = "NaN", strategy = "mean", axis = 0)
imputer = imputer.fit(X[ : , 1:3])
X[ : , 1:3] = imputer.transform(X[ : , 1:3])
print(X)

output : 

[['France' 44.0 72000.0]
D:\:DeprecationWarning: Class Imputer is deprecated; Imputer was deprecated in version 0.20 and will be removed in 0.22. Import impute.SimpleImputer from sklearn instead. warnings.warn(msg, category=DeprecationWarning)
[['France' 44.0 72000.0]
 ['Spain' 27.0 48000.0]
 ['Germany' 30.0 54000.0]
 ['Spain' 38.0 61000.0]
 ['Germany' 40.0 63777.77777777778]
 ['France' 35.0 58000.0]
 ['Spain' 38.77777777777778 52000.0]
 ['France' 48.0 79000.0]
 ['Germany' 50.0 83000.0]
 ['France' 37.0 67000.0]]
 
````

