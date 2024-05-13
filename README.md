# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

1.Import pandas

2.Import Decision tree classifier

3.Fit the data in the model

4.Find the accuracy score 

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: PADMASHREE R
RegisterNumber:  212222040110
*/
import pandas as pd
data=pd.read_csv("/content/Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
x=data[["Position","Level"]]
x.head()
y=data["Salary"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_pred) 
mse
r2=metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])
```

## Output:
### Data.head()
![image](https://github.com/AkilaMohan/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119393915/67b95a8b-2b2c-4a9e-8307-6c1e8e187b1b)

### Data.info()
![image](https://github.com/AkilaMohan/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119393915/9e2c0daf-9f19-403e-825e-852efe176394)

### Data.isnull() and sum()
![image](https://github.com/AkilaMohan/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119393915/660ed4e8-54b1-4eb7-81cd-e8d5a9f11236)

### data.head() for salary
![image](https://github.com/AkilaMohan/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119393915/d08e24a8-e49c-4afc-a6a7-1db14b9ae717)

### MSE
![image](https://github.com/AkilaMohan/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119393915/104530d9-6b7a-48c0-8efa-c46d2f70c60b)

### r2 value
![image](https://github.com/AkilaMohan/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119393915/62febdbc-894d-4189-865f-fbe73509868c)

### data prediction
![image](https://github.com/AkilaMohan/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119393915/f935c9f7-bdb0-4912-bcee-b366b38523bf)


## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
