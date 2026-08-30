# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:

### step 1: Initialize the data – Input the independent variables \(X_1, X_2, ..., X_n\) and dependent variable \(Y\).
### step 2: Initialize coefficients – Set \(b_0, b_1, b_2, ..., b_n\) to initial values (usually 0).
### step 3: Train the model – Calculate predicted value Y^=b0​+b1​X1​+b2​X2​+⋯+bn​Xn​and adjust the coefficients to minimize the Mean Squared Error (MSE).

### step 4: Predict output – Use the trained coefficients with new input values to calculate the predicted \(Y\).

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car.csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression = linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print("Predicted Value:",regression.predict([[3300,1300]]))

```
## Output:

### Insert your output
<img width="1460" height="482" alt="Screenshot 2026-08-30 125207" src="https://github.com/user-attachments/assets/c2a4e868-a459-4862-ad20-b853595cc7ea" />



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
