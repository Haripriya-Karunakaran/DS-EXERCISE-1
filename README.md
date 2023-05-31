# DS-EXERCISE-1  Data Cleaning

## AIM:

To read the given data and perform data cleaning and save the cleaned data to a file.

## EXPLANATION: 

Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect, incompleted ,irrelevant , duplicated or improperly

formatted. Data cleaning is not simply about erasing data, but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

## ALGORITHM:

STEP 1: Read the given Data.

STEP 2: Get the information about the data.

STEP 3: Remove the null values from the data.

STEP 4: Save the Clean data to the file.

## CODE:

import pandas as pd

df=pd.read_csv("Loan_data.csv")

print(df)

df.head(10)

df.info()

df.isnull()

df.isnull.sum()

df['Gender']=df['Gender'].fillna(df['Gender'].mode()[0])

df['Dependents']=df['Dependents'].fillna(df['Dependents'].mode()[0])

df['Self_Employed']=df['Self_Employed'].fillna(df['Self_Employed'].mode()[0])

df.head()

df['LoanAmount']=df['LoanAmount'].fillna(df['LoanAmount'].mean())

df['Loan_Amount_Term']=df['Loan_Amount_Term'].fillna(df['Loan_Amount_Term'].mean())

df.head()

df['Credit_History']=df['Credit_History'].fillna(df['Credit_History'].median())

df.head()

df.info()

df.isnull.sum()

## OUTPUT :

![image](https://github.com/Haripriya-Karunakaran/DS-EXERCISE-1/assets/126390051/591e4dee-d61d-4648-be2f-6bb5f7e0f854)

![image](https://github.com/Haripriya-Karunakaran/DS-EXERCISE-1/assets/126390051/f38d18d9-2835-461f-b5f2-e32a8d66e1f6)

![image](https://github.com/Haripriya-Karunakaran/DS-EXERCISE-1/assets/126390051/9ace95a0-19b6-4a0e-94bd-deb3c6fe7cd1)

![image](https://github.com/Haripriya-Karunakaran/DS-EXERCISE-1/assets/126390051/8b060181-398f-4b33-87a3-43590c05fba9)

![image](https://github.com/Haripriya-Karunakaran/DS-EXERCISE-1/assets/126390051/69fbd60f-5fb1-4f94-9855-afe227f036de)

![image](https://github.com/Haripriya-Karunakaran/DS-EXERCISE-1/assets/126390051/b1671830-3b88-4a16-915c-38846cc36966)

![image](https://github.com/Haripriya-Karunakaran/DS-EXERCISE-1/assets/126390051/a70c056e-1c38-45ce-bf21-38f41d4bacdd)

![image](https://github.com/Haripriya-Karunakaran/DS-EXERCISE-1/assets/126390051/ece307d2-21b6-4b06-b0de-29d2c9372f57)

## RESULT:

Thus, the given data is read, cleansed and the cleansed data is saved into file.
