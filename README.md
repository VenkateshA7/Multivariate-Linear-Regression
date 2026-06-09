# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>Import the required libraries numpy and matplotlib.

### Step2
<br>Define the input data values for X and Y using NumPy arrays.

### Step3
<br>Calculate the mean of X and Y, then find the slope (m) and intercept (c) of the regression line.

### Step4
<br>Predict the output values using the equation:

Y=mX+c

### Step5
<br>Display the original data points and regression line using scatter plot and line plot.

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)




```
## Output:
<img width="795" height="123" alt="image" src="https://github.com/user-attachments/assets/75ed4240-241e-4cd1-92b1-bf0069937d24" />



### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
