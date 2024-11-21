# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

Load and inspect the dataset (Employee.csv) to understand its structure and check for missing values.

Encode categorical variables, such as "salary," to prepare the data for modeling.

Split the data into training and testing sets with an 80-20 ratio.

Train a DecisionTreeClassifier using the "entropy" criterion on the training data.

Evaluate model accuracy and make predictions on test data and a sample input.
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

## Accuracy
![image](https://github.com/user-attachments/assets/b69beca7-bed0-44d4-a60c-71a62b88b26f)

## Predicted
![image](https://github.com/user-attachments/assets/86ae29a7-676e-43cd-9535-d547613979ae)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
