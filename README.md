# workshop-Multivariate-analysis
# Aim
To perform Multivariate EDA on the given data set.

# Explanation
Exploratory data analysis is used to understand the messages within a dataset. This technique involves many iterative processes to ensure that the cleaned data is further sorted to better understand the useful meaning.The primary aim with exploratory analysis is to examine the data for distribution, outliers and anomalies to direct specific testing of your hypothesis.

# Algorithm
# Step1
Import the built libraries required to perform EDA and outlier removal.

# Step2
Read the given csv file.

# Step3
Convert the file into a dataframe and get information of the data.

# Step4
Return the objects containing counts of unique values using (value_counts()).

# Step5
Plot the counts in the form of Histogram or Bar Graph.

# Step6
Use seaborn the bar graph comparison of data can be viewed.

# Step7
Find the pairwise correlation of all columns in the dataframe.corr()

# Step8
Save the final data set into the file.

# Types of bivariate analyis

1)Numerical & Numerical(Scatter plot)

2)Numerical & Categorical(Bar plot,Box plot,Dist plot)
# Code
Developed by : SHARANGINI T K

Registration Number : 212222230143
```
import pandas as pd
import numpy as py
import seaborn as sns
import matplotlib.pyplot as plt

df=pd.read_csv('FlightInformation (1).csv')sns.scatterplot(df['Duration'],df['Price'],hue=df['Dep_Time'])
df
df.head()
df.info()
df.describe()
df.isnull().sum()
df.dtypes

sns.scatterplot(df['Duration'],df['Price'],hue=df['Dep_Time'])
sns.barplot(x=df['Dep_Time'],y=df['Price'],data=df)
df.corr()
```
# Output

# Data Head
![image](https://user-images.githubusercontent.com/113497104/229035875-18448918-4fd1-4958-8e34-c84e83f3ce00.png)

# Data Information
![image](https://user-images.githubusercontent.com/113497104/229036027-ae28fc92-fd7b-4d9a-88b9-701234551c1d.png)

# Numerical & Numerical(Scatter plot)
![image](https://user-images.githubusercontent.com/113497104/229036100-9ff854e8-bbcf-42df-ba79-f703da0eadd0.png)

# Numerical & Categorical(Bar plot)
![image](https://user-images.githubusercontent.com/113497104/229036194-b70cb7e9-afd6-41ac-97dd-4f43bd3fb975.png)

# Non-Graphical method(correlation)
![image](https://user-images.githubusercontent.com/113497104/229036249-6dd6bd41-71df-46b0-9770-298d6a0c6e49.png)

# Result
Thus we have performed Multivariate EDA on the given data set.

