# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>

### Step2
<br>

### Step3
<br>

### Step4
<br>

### Step5
<br>

## Program:
```
import numpy as np
import matplotlib.pyplot as plt

# Preprocessing Input data
X = np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
Y = np.array([1, 3, 2, 5, 7, 8, 8, 9, 10, 12])

plt.scatter(X, Y)
plt.show()

# Building the model
X_mean = np.mean(X)
Y_mean = np.mean(Y)

num = 0
den = 0

for i in range(len(X)):
    num += (X[i] - X_mean) * (Y[i] - Y_mean)
    den += (X[i] - X_mean) ** 2

m = num / den
c = Y_mean - m * X_mean

print(m, c)

# Making predictions
Y_pred = m * X + c
print(Y_pred)

plt.scatter(X, Y)
plt.scatter(X, Y_pred, color='red')
plt.plot([min(X), max(X)], [min(Y_pred), max(Y_pred)],
         color='red')  # predicted

plt.show()





```
## Output:
<img width="703" height="521" alt="image" src="https://github.com/user-attachments/assets/ff475214-9639-48f0-b05a-1ff381bbbe10" />
<img width="770" height="112" alt="image" src="https://github.com/user-attachments/assets/03f16e60-4aee-4623-8cc5-ea4d5312361a" />
<img width="698" height="526" alt="image" src="https://github.com/user-attachments/assets/a5d7235e-0c79-46ec-8b05-435bdb00e63c" />


### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
