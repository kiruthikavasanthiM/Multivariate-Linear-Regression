# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## step1: Import the required libraries and load the California Housing dataset
## step2: Define the feature matrix X and target vector y.
## step3: Split the dataset into training and testing sets using train_test_split().
## step4: Create and train the Linear Regression model using the training data.
## step5: Predict the output, calculate the variance score, and plot the residual errors.
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

<img width="1460" height="482" alt="Screenshot 2026-08-30 125207" src="https://github.com/user-attachments/assets/8f32d29c-ea29-4bbd-aced-bc78103cabd4" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
