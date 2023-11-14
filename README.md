# Ex 03 Univariate-Analysis
## Aim:
To read the given data and perform the univariate analysis with different types of plots.
## Explanation:
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means
that the data has only one kind of variable. The major reason for univariate analysis is to use the
data to describe. The analysis will take data, summarise it, and then find some pattern in the data.
## Algorithm:
Step 1: Read the given data.<br/>
Step 2: Get the information about the data.<br/>
Step 3: Remove the null values from the data.<br/>
Step 4: Mention the datatypes from the data.<br/>
Step 5: Count the values from the data.<br/>
## Program:
```
Developed By : ANISHRAJ P
Register Number: 212222230010
```
## Superstore.csv
```
import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv('SuperStore.csv')
print(df)
df.head()
df.info()
df.dtypes
df['Postal Code'].value_counts()
sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
df.describe()
```
## Diabetes.csv
```
import pandas as pd
import numpy as np
import seaborn as sns
df = pd.read_csv("/diabetes.csv")
df
df.info()
df.isnull().sum()
df.dtypes
df.describe()
df['Glucose'].value_counts()
sns.boxplot(x="Glucose",data=df)
sns.countplot(x="Glucose",data=df)
sns.distplot(df['Glucose'])
sns.histplot(x="Glucose",data=df)
df.skew()
df.kurtosis()
```
## OUTPUT:
### Superstore.csv
![Superstore.csv](1.png)<br/>
![Superstore.csv](2.png)<br/>
![Superstore.csv](3.png)<br/>
![Superstore.csv](4.png)<br/>
![Superstore.csv](5.png)<br/>
![Superstore.csv](6.png)<br/>
![Superstore.csv](7.png)<br/>
![Superstore.csv](8.png)<br/>
![Superstore.csv](9.png)<br/>
### Diabetes.csv
![Diabetes.csv](10.png)<br/>
![Diabetes.csv](11.png)<br/>
![Diabetes.csv](12.png)<br/>
![Diabetes.csv](13.png)<br/>
![Diabetes.csv](14.png)<br/>
![Diabetes.csv](15.png)<br/>
![Diabetes.csv](16.png)<br/>
![Diabetes.csv](17.png)<br/>
![Diabetes.csv](18.png)<br/>
![Diabetes.csv](19.png)<br/>
![Diabetes.csv](20.png)<br/>
![Diabetes.csv](21.png)<br/>
## RESULT:
### Thus the univariate analysis is verified with the help of different plots.
