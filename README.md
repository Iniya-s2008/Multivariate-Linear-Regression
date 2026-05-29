# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
Step1
Import the required libraries such as pandas and LinearRegression.

Step2
Read the dataset from the CSV file and store it in a dataframe.

Step3
Select the input features (Volume, Weight) and output variable (CO2).

Step4
Create and train the Linear Regression model using the training data.

Step5
Display the coefficient, intercept, and predict the CO2 emission for the given input values [3300,1300].

## Program:
```
#DEVELOPED BY : INIYA S
#REGISTER NUMBER :212225230104

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car (1).csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))










```
## Output:

### Insert your output

<img width="1407" height="410" alt="exp10multi" src="https://github.com/user-attachments/assets/ae5f033c-0736-499d-8bad-ea3ae8d27b13" />


<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
