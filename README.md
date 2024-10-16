# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

Import the required libraries.
Upload and read the dataset.
Check for any null values using the isnull() function.
From sklearn.tree import DecisionTreeClassifier and use criterion as entropy.
Find the accuracy of the model and predict the required values by importing the required module from sklearn.
## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: LATHIKA L J
RegisterNumber:  212223220050

import pandas as pd

data=pd.read_csv("/content/Employee.csv")

data.head()

data.info()

data.isnull().sum()

data["left"].value_counts()

from sklearn.preprocessing import LabelEncoder le=LabelEncoder()

data["salary"]=le.fit_transform(data["salary"])

data.head()

x=data[["satisfaction_level", "last_evaluation", "number_project","average_montly_hours", "time_spend_company", "Work_accident", "promotion_last_5years", "salary"]]

x.head(

y=data["left"]

from sklearn.model_selection import train_test_split

x_train, x_test,y_train,y_test=train_test_split(x, y, test_size=0.2, random_state=100)

from sklearn.tree import DecisionTreeClassifier dt=DecisionTreeClassifier (criterion="entropy") dt.fit(x_train, y_train) y_pred=dt.predict(x_test)

from sklearn import metrics

accuracy=metrics.accuracy_score(y_test,y_pred)

dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```

## Output:
![image](https://github.com/user-attachments/assets/6d1dd711-9d63-4539-9809-1aa0f05cc6e3)

![image](https://github.com/user-attachments/assets/cc1bd304-8cdf-435b-b452-a16352df1a49)
![image](https://github.com/user-attachments/assets/181bb4ea-caac-409e-9358-1289b639b7c3)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
