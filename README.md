# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. import the required libraries.


2.Upload and read the dataset.


3.Check for any null values using the isnull() function.


4.From sklearn.tree import DecisionTreeClassifier and use criterion as entropy.


5.Find the accuracy of the model and predict the required values by importing the required module from sklearn.

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: DIVAKAR R
RegisterNumber: 212222240026

import pandas as pd
data=pd.read_csv("Employee.csv")
data.head()

data.info()

data.isnull().sum()

data["left"].value_counts()

from sklearn.preprocessing import LabelEncoder 
le=LabelEncoder()

data["salary"]=le.fit_transform(data["salary"])
data.head()

x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()

y=data["left"]

from sklearn.model_selection import train_test_split
x_train, x_test, y_train, y_test = train_test_split(x,y,test_size=0.2, random_state=100)

from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test, y_pred)
accuracy

dt.predict([[0.5, 0.8, 9, 260, 6, 0, 1, 2]])
*/
```

## Output:
data.head()
![ml601](https://github.com/divakar618/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118708040/a018a537-df44-433a-9009-9e128bdd7bd6)
data.info()

![ml602](https://github.com/divakar618/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118708040/a45b594a-a9de-413d-9e49-2a8b09b5c5ef)


isnull() and sum()


![ml603](https://github.com/divakar618/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118708040/0502bf8f-85f2-48eb-be75-db41e46aa07c)


data value counts()


![ml604](https://github.com/divakar618/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118708040/90f20e9e-9b79-4abd-afb6-972bd0fb72df)


data.head() for salary


![ml605](https://github.com/divakar618/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118708040/db5fde9c-1c37-4622-a6ac-aa8a7f9eae45)


x.head()

![ml606](https://github.com/divakar618/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118708040/cee35c78-1839-4025-aad1-03ca90e4d78f)


accuracy value:

![ml607](https://github.com/divakar618/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118708040/d1dda193-484c-46b7-b075-aeadb1760465)


data prediction:

![ml608](https://github.com/divakar618/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118708040/1774dcdb-6170-416b-8ee5-8781c931fa92)





## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
