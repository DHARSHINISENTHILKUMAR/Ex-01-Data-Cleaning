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
### import pandas as pd df=pd.read_csv("/content/Data_set.csv") print(df) df.head(5) df.info() df.isnull().sum() df['show_name']=df['show_name'].fillna(df['aired_on'].mode()[0]) df['aired_on']=df['aired_on'].fillna(df['aired_on'].mode()[0]) df['original_network']=df['original_network'].fillna(df['aired_on'].mode()[0]) df.head() df['rating']=df['rating'].fillna(df['rating'].mean()) df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mean()) df.head() df['watchers']=df['watchers'].fillna(df['watchers'].median()) df.head() df.info() df.isnull().sum()

# OUPUT
### ![image](https://user-images.githubusercontent.com/113699377/226260915-97b4487b-e170-4640-a36b-31a64582ced7.png)
## df.head()
### ![image](https://user-images.githubusercontent.com/113699377/226261014-3e9cb83d-0088-431b-a7e0-81ae8807c247.png)
## df.info()
### ![image](https://user-images.githubusercontent.com/113699377/226261092-402c1ad7-2e1c-4970-964e-6d9eb4f6a50b.png)
## df.isnull().sum()
### ![image](https://user-images.githubusercontent.com/113699377/226261189-44330977-45af-43ce-81dc-79c45a67aed7.png)
# Result:
## Hence the given data is read and perform data cleaning and save the cleaned data to a file.


