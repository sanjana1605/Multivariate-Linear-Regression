# Implementation of Multivariate Linear Regression
Date:18-05-2024
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:

## Step1
import pandas as pd.
 
## Step2
Read the csv file.
 
## Step3
Read the csv file.
 
## Step4
Create the linear regression model and fit.
 
## Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.
 
## Program:
```
#Program to find Multivariate linear regression
#Developed By: Sanjana Sri N
#Register Number: 2305003007

import pandas as pd
from sklearn import linear_model
data = pd.read_csv("car.csv")
X = data[['Weight','Volume']]
y = data[['CO2']]
regr = linear_model.LinearRegression()
regr.fit(X,y)
print("coefficients:",regr.coef_)
print("Intercept:",regr.intercept_)
predictCO2 = regr.predict([[3300,1300]])
print("predicted CO2 for the corresponding weight and volume:",predictCO2)
```
## Output:

### Insert your output
![WhatsApp Image 2024-05-26 at 18 55 06_c73cbb56](https://github.com/sanjana1605/Multivariate-Linear-Regression/assets/155608340/6b970345-c241-48b8-96c3-d24b6524b2c1)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
