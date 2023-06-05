# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:

### Step1
import pandas as pd.

### Step2
Read the CSV file

### Step3
Get the value of x and y variables.

### Step4
Create the linear regression model and fit

### Step5
Predict the CO2 emission of a car where the weight is 2300Kg, and the volume is 1300cm3

###Step6
Print the predicted output.

## Program:
```
## Developed by :K.SANTHANA LAKSHMI
## REGISTER NUMBER :212222240091

import pandas as pd
from sklearn import linear_model

data=pd.read_csv("cars.csv")
x=data[['Weight','Volume']]
y=data[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictCO2=regr.predict([[3300,1300]])
print('predicted CO2 for the corresponding weight and volume',predictCO2)

```
## Output:
![image](https://github.com/santhanalakshmi04/Multivariate-Linear-Regression/assets/119475762/ac4b2282-8dd6-4f72-a182-f2ee9c6167d8)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
