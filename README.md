# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the standard Libraries.

2.Set variables for assigning dataset values.

3.Import linear regression from sklearn.

4.Assign the points for representing in the graph.

5.Predict the regression for the marks by using the representation of the graph.

6.Compare the graphs and hence we obtained the linear regression for the given datas


## Program:
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: Siva Chandran R
RegisterNumber: 212222240099
*/
```
```
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
plt.scatter(df['X'],df['Y'])
plt.xlabel('X')
plt.ylabel('Y')
X=df.iloc[:,0:1]
Y=df.iloc[:,-1]
X
from sklearn.model_selection import train_test_split
X_train,X_test,Y_train,Y_test=train_test_split(X,Y,test_size=0.2,random_state=0)
from sklearn.linear_model import LinearRegression
lr=LinearRegression()
lr.fit(X_train,Y_train)
X_train
Y_train
lr.predict(X_test.iloc[0].values.reshape(1,1))
plt.scatter(df['X'],df['Y'])
plt.xlabel('X')
plt.ylabel('Y')
plt.plot(X_train,lr.predict(X_train),color='red')
m=lr.coef_
m[0]
b=lr.intercept_
b
```
## Output:
![image](https://github.com/SivaChandranR07/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/113497395/c8a05c97-2f7a-4294-bf36-5f0a39636a3c)

![image](https://github.com/SivaChandranR07/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/113497395/f452df95-2920-47b6-b387-15b8732aea7b)

![image](https://github.com/SivaChandranR07/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/113497395/3ca65e0b-21a4-4bb9-a743-23fb8aa80b41)


## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
