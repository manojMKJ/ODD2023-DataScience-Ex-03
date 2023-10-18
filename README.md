# ODD2023-DataScience-Ex-03
# Ex-03 Univariate Analysis
# Aim:
To read the given data and perform the univariate analysis with different types of plots.
# Explanation:
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.
# Algorithm:
### Step1:
Read the given data.

### Step2:
Get the information about the data.

### Step3:
Remove the null values from the data.

### Step4:
Mention the datatypes from the data.

### Step5:
Count the values from the data.

### Step6:
Do plots like boxplots,countplot,distribution plot,histogram plot.

# Program:
DEVELOPED BY : Manoj Kumar G
REGISTER NO : 212222230078
## diabetes.csv
```
import pandas as pd
import numpy as np
from scipy import stats
import seaborn as sns

data=pd.read_csv("/content/diabetes.csv")
df=pd.DataFrame(data)

sns.boxplot(data=df)
sns.scatterplot(data=df)

df.info()
df.dtypes
df['BMI'].value_counts()
df.describe

sns.boxplot(x='Age', data=df)
sns.countplot(x="Age", data=df)
sns.distplot(df["Age"])
sns.histplot(x="Age", data=df)

df.skew()
sns.histplot(x="Insulin", data=df)
sns.displot(x="BloodPressure", data=df)

df.kurtosis()
sns.boxplot(x="Glucose",data=df)
```
### Dataset:
![1](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/6daa8e40-dc12-45ab-b296-e97da4d395c5)
### boxplot:
![2](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/33bf405d-c699-4e5b-b3a4-666328a9a1ef)
### scatterplot:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/d3b15366-435a-42eb-8928-be942a2d46a5)
### info:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/2a036502-7b8e-4a12-9759-7a89994d548a)
### Datatypes:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/a59598d6-115f-4ee0-977f-defa893c8952)
### Value counts:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/a5b3f4f9-ca93-4de8-b1e3-35e5f3bb6260)
### describe:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/cad2ed50-a13f-40d2-9994-e411a3474554)
## OUTPUT:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/636ebb4b-0b72-41be-92ea-f81704448dc2)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/acdfe8af-47be-4f7a-b5ab-05fac9a2709e)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/c10a1ff2-52d3-4e3a-968a-a3e77ed3d20f)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/ec717d4f-4f5a-4f37-a758-5458d8c491d9)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/80cd7dc5-8257-44ec-82e7-97fd4be27b1e)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/8200aa79-9b63-4f43-ad35-dbbdf210a5c2)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/50745127-4b36-4e5c-904d-2d4a6ca2c2db)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/8bd93219-868a-4d08-a950-c5722e5c6ec4)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/a811c2c1-1cf9-4c5f-b955-ac4edc4efa79)
## RESULT:
Thus we have read the given data of diabetes.csv and performed the univariate analysis with different types of plots.

## employeesal.csv
```
import pandas as pd
import numpy as np
from scipy import stats
import seaborn as sns

data=pd.read_csv("/content/employeesal.csv")
df=pd.DataFrame(data)

df
sns.boxplot(data=df)
sns.scatterplot(data=df)

df.info()
df.dtypes

df['Age'].value_counts()
df.describe

sns.boxplot(x='Age', data=df)
sns.countplot(x="Age", data=df)
sns.distplot(df["Age"])
sns.histplot(x="Age", data=df)

df.skew()
sns.histplot(x="Salary", data=df)
sns.displot(x="ID", data=df)

df.kurtosis()
sns.boxplot(x="ID",data=df)
```
### Dataset:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/f56d6c8f-6b5d-41f9-9b28-f1e4107e1355)
### boxplot:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/bc129a22-c91c-4764-89dc-65874922c2fa)
### scatterplot:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/efab534d-2df5-439e-b352-defeb01537f1)
### info:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/bca8a694-6a19-4c24-a771-b00c091aa4a7)
### Datatypes:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/84a1b03a-c316-4e50-9a34-84ae00081a8e)
### Value counts:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/976e56d8-3730-45d6-920b-fda47e453740)
### describe:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/89db2678-bb41-45cf-970f-6457411a7619)

## OUTPUT:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/f9ad02fb-6e45-488e-aea7-01b98f60bd62)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/5e47de69-2338-40b4-b7ea-932f7e6f40bb)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/577f0fad-430c-4b72-8c46-9ef0ff52b59a)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/e8577501-d620-4cef-b3eb-e081a7ba8e49)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/fcd0bec7-bffc-4c58-83ae-e902db9a5153)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/c88fdceb-bc49-4af9-9e8c-5723ad5a66e9)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/1bc547e9-3f15-4222-88d8-3f3d4d634d27)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/968bc7d6-5326-4389-bca2-d2ec62ddb12e)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/997c393b-9977-4385-a89c-79f879fd6230)

## RESULT:
Thus we have read the given data of employeesal.csv and performed the univariate analysis with different types of plots.

## SuperStore.csv
```
import pandas as pd
import numpy as np
from scipy import stats
import seaborn as sns

data=pd.read_csv("/content/SuperStore.csv")
df=pd.DataFrame(data)

df
sns.boxplot(data=df)
sns.scatterplot(data=df)

df.info()
df.dtypes
df['City'].value_counts()
df.describe()

sns.boxplot(x='Row ID', data=df)
sns.countplot(x="Postal Code", data=df)
sns.distplot(df["Row ID"])
sns.histplot(x="Postal Code", data=df)

df.skew()
sns.histplot(x="Postal Code", data=df)
sns.displot(x="City", data=df)

df.kurtosis()
sns.boxplot(x="Postal Code",data=df)
```
### Dataset:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/347ebb67-bba8-4995-8a30-8f8e01bb5724)
### boxplot:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/1974982f-000e-4af0-a5cb-4ff4b9330c7a)
### scatterplot:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/6fc7aa15-0a7f-479c-a320-ffbd0220cb67)
### info:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/0e05ec08-e06a-497c-b0b0-797ea3d7676b)
### Datatypes:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/d6b04f68-9d67-4bfc-b67e-da6de037963a)
### Value counts:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/1c236778-3a43-4dca-a4e2-8ac39b7d8518)
### describe:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/cd21e80d-1bd8-427a-92a7-70a69aeeb0c2)

## OUTPUT:
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/c46f8d81-fde0-4098-beda-ad919f9f71ce)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/5bc00c2d-663d-41ad-a860-d77240941d0d)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/11b021cc-7f00-456b-9cea-3892ff67882a)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/86112ad3-ee80-41bb-b7e6-1e88e8cbda71)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/764dc951-2740-4b07-b4cc-b3cab94b4969)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/401ac88a-804a-4984-a9c6-ea6f42cc40ca)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/01e9d1f8-4373-41c4-8ea6-97baf70a154e)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/b8186bad-310b-4a3c-99e3-87759ca137cd)
![image](https://github.com/ASHWINKUMAR2903/ODD2023-DataScience-Ex-03/assets/119407186/6d1e2edd-49ab-4b45-ba58-76890f6f5c33)

## RESULT:
Thus we have read the given data of SuperStore.csv and performed the univariate analysis with different types of plots.
