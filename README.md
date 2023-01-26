# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd

### Step2
Read csv file

### Step3
Get the value of X and y variables

### Step4
Create the linear regresssion model and fit

### Step5
Predict the CO2 emission of a car wher the weight is 1000kg,and the volume is 1390cm3

###Step6
Print the predict output

## Program:
```
#developed by S.Subashini
#Refernce no:22009344
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car.csv")
x=df[['Weight','Volume']]
y=df['Co2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCo2=regr.predict([[3300,1300]])
print("Predicted Co@ for the corresponding weight and volume",predictedCo2)






```
## Output:

![multivarient](https://user-images.githubusercontent.com/119404951/214741877-130e764e-17d8-4eb5-a205-88d2e9454e9b.png)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
