## Sales Prediction using Linear Regression

### Problem Statement

Build a model which predicts sales based on the money spent on different platforms for marketing.

### Data
Use the advertising dataset given in ISLR and analyse the relationship between 'TV advertising' and 'sales' using a simple linear regression model. 

In this notebook, we'll build a linear regression model to predict `Sales` using an appropriate predictor variable.

## Checking Null values
There are no NULL values in the dataset, hence it is clean.

### Outlier Analysis
![image](https://user-images.githubusercontent.com/22324848/188295143-34f654fc-ad7b-43f4-8a85-f6f78ed0d466.png)

There are no considerable outliers present in the data.

### Univariate Analysis

![image](https://user-images.githubusercontent.com/22324848/188295161-7afd6470-891b-450c-ad25-1ebc11c5ebda.png)

![image](https://user-images.githubusercontent.com/22324848/188295164-26241a82-1c86-43bc-9656-ad4a0c7f3dd3.png)

![image](https://user-images.githubusercontent.com/22324848/188295176-faa95e8a-4f13-49b5-8794-67c367f6e3ca.png)

As is visible from the pairplot and the heatmap, the variable TV seems to be most correlated with Sales. 
So let's go ahead and perform simple linear regression using TV as our feature variable.


## Linear Regression

Equation of linear regression<br>
$y = c + m_1x_1 + m_2x_2 + ... + m_nx_n$

-  $y$ is the response
-  $c$ is the intercept
-  $m_1$ is the coefficient for the first feature
-  $m_n$ is the coefficient for the nth feature<br>

In our case:

$y = c + m_1 \times TV$

The $m$ values are called the model **coefficients** or **model parameters**.


![image](https://user-images.githubusercontent.com/22324848/188295209-54e736ce-aae4-4957-8dce-77fc37a2e931.png)

![image](https://user-images.githubusercontent.com/22324848/188295228-f3336947-decc-4af8-a545-a111af23e007.png)

The residuals are following the normally distributed with a mean 0. All good!

![image](https://user-images.githubusercontent.com/22324848/188295237-397dfa13-e488-4bae-bf94-86f59ce9b152.png)

We are confident that the model fit isn't by chance, and has decent predictive power. The normality of residual terms allows some inference on the coefficients.

Although, the variance of residuals increasing with X indicates that there is significant variation that this model is unable to explain.


![image](https://user-images.githubusercontent.com/22324848/188295245-18630b05-ebce-4585-a4b0-8f94504bd2ce.png)
