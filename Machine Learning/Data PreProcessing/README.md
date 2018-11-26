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
X = dataset.iloc[ : , :-1].values
Y = dataset.iloc[ : , 3].values

````


