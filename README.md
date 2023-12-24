# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Step 1:
import pandas as pd.

## Step 2:
Read the CSV file.

## Step 3:
Get the value of x and y variables.

## Step 4:
Create the linear regression model and fit.

## Step 5:
Predict the CO2 emission of a car where the weight is 2300Kg, and the volume is 1300cm3.

## Step 6:
Print the predicted output.

### Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("/content/cars (1).csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO@ for the corresponding weight and volume",predictedCO2)
```

## Output:
```
Coefficient: [0.00755095 0.00780526]
Intercept: 79.69471929115939
Predicted CO@ for the corresponding weight and volume [114.75968007]
```
### Insert your output

![Screenshot 2023-12-24 200802](https://github.com/etjabajasphin/Multivariate-Linear-Regression/assets/151705853/045817bb-eb2d-4e18-854e-06bd3312504f)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
