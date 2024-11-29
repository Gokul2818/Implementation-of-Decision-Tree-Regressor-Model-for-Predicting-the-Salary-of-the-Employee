# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import pandas
2. Import Decision tree classifier
3. Fit the data in the model
4. Find the accuracy score

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: GOKUL S
RegisterNumber:  24004336
import pandas as pd
data=pd.read_csv("Salary.csv")
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
y.head()

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
x_train

from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_pred)
mse

r2=metrics.r2_score(y_test,y_pred)
r2

dt.predict([[5,6]])
*/
```
## Output:
INFO:

![image 1](https://github.com/user-attachments/assets/ffbdda5c-dcb6-41bd-8b95-67e2ca4f3be7)

HEAD:

![image 2](https://github.com/user-attachments/assets/7878d9c8-e944-4958-8761-b6909be82296)

POSITION:

![image 3](https://github.com/user-attachments/assets/3daf3347-60d9-4ec4-9a32-64bf7bd31e47)

SALARY:

![image 4](https://github.com/user-attachments/assets/eb896f69-8c3f-4d40-8298-e7b29b6e95b7)

SELECTION:

![image 5](https://github.com/user-attachments/assets/dd9061b3-44a0-47e2-97fc-95d917aa5d82)

MSE:

![i 6](https://github.com/user-attachments/assets/5e8db707-0edb-4378-8d51-0d69fff5aa05)

PREDICTION:

![i 7](https://github.com/user-attachments/assets/a5f37399-2961-478d-901f-54de70b2c1eb)


![i 8](https://github.com/user-attachments/assets/783dd6ae-e812-4ffa-8920-daa399c56da3)
## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
