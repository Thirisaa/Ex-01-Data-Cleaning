# Ex-01_DS_Data_Cleansing
# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# ALGORITHM
## STEP 1
Read the given Data

## STEP 2
Get the information about the data

## STEP 3
Remove the null values from the data

## STEP 4
Save the Clean data to the file

# CODE
import pandas as pd

df=pd.read_csv('/content/Data_set.csv')

df.head() 

df.isnull().sum()

df['show_name']=df['show_name'].fillna(df['show_name'].mode()[0])

df['aired_on']=df['aired_on'].fillna(df['aired_on'].mode()[0])

df['original_network']=df['original_network'].fillna(df['original_network'].mode()[0])

df.head()

df['rating']=df['rating'].fillna(df['rating'].mean())

df['watchers']=df['watchers'].fillna(df['watchers'].mean())

df.head()

df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].median())

df.head()

df.isnull().sum()

df=pd.read_csv('/content/Loan_data.csv')

df.head()

df.isnull().sum()

df['Gender']=df['Gender'].fillna(df['Gender'].mode()[0])

df['Dependents']=df['Dependents'].fillna(df['Dependents'].mode()[0])

df['Self_Employed']=df['Self_Employed'].fillna(df['Self_Employed'].mode()[0])

df.head()

df['LoanAmount']=df['LoanAmount'].fillna(df['LoanAmount'].mean())

df.head()

df['Loan_Amount_Term']=df['Loan_Amount_Term'].fillna(df['LoanAmount'].median())

df['Credit_History']=df['Credit_History'].fillna(df['Credit_History'].median())

df.head()

df.isnull().sum()

# OUPUT
![op1](https://user-images.githubusercontent.com/112301582/226176454-3e1b37ea-54d3-4c16-9102-e75b34ecf6aa.png)
![op2](https://user-images.githubusercontent.com/112301582/226176520-88a9f6f8-81f7-48bd-bc8c-b8eb4fd8bf75.png)
![op3](https://user-images.githubusercontent.com/112301582/226176531-f922bd6f-1bc5-4655-a6fa-51ba2ca8c380.png)
![op4](https://user-images.githubusercontent.com/112301582/226177262-31f8f842-cc62-44aa-8e13-745fa5051a66.png)
![op5](https://user-images.githubusercontent.com/112301582/226176548-a67711f9-85be-4631-9f5e-d664971314dd.png)
![op6](https://user-images.githubusercontent.com/112301582/226176560-fe2d657f-f933-4a02-81bd-98d580d0befc.png)
![op7](https://user-images.githubusercontent.com/112301582/226177279-ab9e8226-d4d9-4e93-a72d-c86b9b13d97f.png)
![op8](https://user-images.githubusercontent.com/112301582/226176984-fc268bb7-c404-4502-a415-84678fa74031.png)
![op9](https://user-images.githubusercontent.com/112301582/226176990-900d024d-e703-4287-9eae-0370c7fce4da.png)
![op10](https://user-images.githubusercontent.com/112301582/226176995-f9495626-3105-4dce-8774-ea64689a7c74.png)
![op11](https://user-images.githubusercontent.com/112301582/226177422-ba559bb6-69c8-4689-b61f-1ff15c45619c.png)
![op12](https://user-images.githubusercontent.com/112301582/226177010-8501c40e-ae78-4331-9cd7-1250363e2824.png)

#RESULT

Thus the given data is read,data cleaning is performed on it and the cleaned data is saved into the file.







