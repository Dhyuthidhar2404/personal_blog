---
title: Mastering Linear Regression: From Basics to Gradient Descent
date: 2024-01-06T09:09:32.780228
---

## Introduction

Linear regression is a machine learning model used to predict the input by learning and analyzing some data. This blog will explore linear regression from the basics to the advanced level.

## What is Regression?

It is a statistical representation of the relationship between dependent and independent variables. It will tell how the dependent variables relate to the independent variables. It is used for predicting the value of the dependent variable using all independent variables. There are many types of regression techniques but the most common one is Linear Regression.

## What is Linear Regression?

It is a Supervised Machine Learning Algorithm that tells the relationship between the dependent and independent variables. It assumes that the relation between these variables is a straight line. It takes the independent variable's data points and predicts the value of the dependent variable using that graph. The output of linear regression will be in a continuous form i.e. numerical value. For example, the output can be height, weight, age, revenue of the company, etc.

## Importance of Linear Regression -:

Many applications can be done because of linear regression including knowing the relationship between independent and dependent variables and prediction purposes, which helps in predicting the new value in the dependent variable. Linear regression can also be used for feature selection. Linear regression is used in medical fields and financial fields to predict stock prices etc.

## Mathematical Understanding of Linear Regression -:

We will make a linear regression model so that it will find the best-fit line that covers all the data points and helps us with prediction. As it is a line the formula for the straight line is y = mx + c. Here m is the slope of the line and c is the intercept of the line.

Based on the equation you will get the predicted values and the distance between the predicted values and original values should be less. So the difference between those two points is known as error. If the error is the least then it is the best-fit line.

## Cost Function

It is also known as loss function and mean squared error. The function is based on the error which is y(predicted) - y(actual).

J(\theta) = \frac{1}{2m} \sum_{i=1}^{m} (h_\theta(x^{(i)}) - y^{(i)})^2

In this equation hθ​(x(I)) is the predicted value and y(I) is the actual value and the difference between them will be the error. We are squaring the error as there will be negative error or positive error and we will add all of them.

We are dividing by m to get the average of that value and dividing with 2 as it will be used for the derivation of the function.

Guess where we will use the derivative of this function?😉. You will get the answer in the next topic.

Our job is to minimize this function so that the distance between the predicted and actual value decreases and we will get the best fit line.

How can we decrease this cost function?🤔

Here comes the topic of gradient descent. Which is a very important topic in machine learning.

## Gradient Descent -:

You will find this topic also in deep learning that is when we are discussing neural networks.

if you are interested wait for my upcoming blogs.😉

Here we will compare the cost function with two hyperparameters which are slope and intercept (m, c).

Gradient descent plays a crucial role in finding the correct values of m and c so that the loss function value will be low and the best values for those two are at the Global Minima.

We will find the derivative of the loss function so that we can find the slope. And while doing the derivative of the loss function as I mentioned before 1/2 in the loss function helps as the derivative of square is 2 will be multiplied with error and this 2 gets cancelled by that 1/2.

\frac{\partial J(\theta)}{\partial \theta_j} = \frac{1}{m} \sum_{i=1}^{m} (h_\theta(x^{(i)}) - y^{(i)}) \cdot x_j^{(i)}

You can see in the above formula which is the derivative of the loss function.

Gradient descent is an iterative algorithm, you have to run this many times to get the best result which is the least loss and we will find the values of m and c where the loss is least using gradient descent.

So using the derivative we found the direction in which the point should move so that it comes near to the global minima but we didn't mention the step length which is how big a step it should take to go towards the global minima, to solve this problem there is another parameter in the gradient descent algorithm which is Learning Rate.

As the Learning Rate is higher the point takes a big step towards the global minima and if the Learning Rate is lower the point takes small steps towards the global minima.

Learning Rate is most commonly denoted by the Greek letter alpha(α).

\theta_j := \theta_j - \alpha \frac{\partial J(\theta)}{\partial \theta_j}

You can see in the above formula θj can be either m or c and α is the learning rate which is multiplied by the derivative of the loss function wrt either m or c.

m= m - \alpha \frac{1}{m} \sum_{i=1}^{m} (h_\theta(x^{(i)}) - y^{(i)}) \cdot x^{(i)}

c = c - \alpha \frac{1}{m} \sum_{i=1}^{m} (h_\theta(x^{(i)}) - y^{(i)})

These two are the changes which we make in the gradient descent algorithm for the hyperparameters of linear regression.

Here is the simpler version of those two formulas:

## Conclusion

As we come to the end of our investigation of linear regression, from its fundamental ideas to the particulars of gradient descent, I kindly encourage you to participate in this educational experience. Please leave your questions, comments, and views below😉. Your engaged involvement enhances our educational process and creates the foundation for the next conversations.

Participate in the discussion by sharing your thoughts, posing questions, or suggesting subjects for future blogs. Let's work together to create a thriving learning community that encourages cooperation and exploration. Cheers to many more adventures ahead!😁