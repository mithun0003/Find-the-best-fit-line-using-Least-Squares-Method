Implementation of Univariate Linear Regression


AIM:
To implement univariate Linear Regression to fit a straight line using least squares.


Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

Algorithm:

1. Get the independent variable X and dependent variable Y.
2. Calculate the mean of the X -values and the mean of the Y -values.
3. Find the slope m of the line of best fit using the formula.


![image](https://github.com/user-attachments/assets/897b897f-57cb-494b-a9ae-e3570c365025)

5. Compute the y -intercept of the line by using the formula:


![image](https://github.com/user-attachments/assets/f9b8d198-5361-4063-82af-f607fb4e7a7d)

7. Use the slope m and the y -intercept to form the equation of the line.
8. Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
```
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by:MITHUN G
RegisterNumber:212223080030

import numpy as np
import matplotlib.pyplot as plt
X=np.array(eval(input()))
Y=np.array(eval(input()))
X_mean=np.mean(X)
print(X_mean)
Y_mean=np.mean(Y)
print(Y_mean)
num=0
denum=0
for i in range(len(X)):
  num+=(X[i]-X_mean)*(Y[i]-Y_mean)
  denum+=(X[i]-X_mean)**2
m=num/denum
print(m)
b=Y_mean - m*X_mean
print(b)
Y_pred=m*X+b
print(Y_pred)
plt.scatter(X,Y,color='blue')
plt.plot(X,Y_pred,color='yellow') 
plt.show() 
```
## Output:

![image](https://github.com/user-attachments/assets/1448efbe-809b-4a84-9dd0-927875ec823f)




## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
