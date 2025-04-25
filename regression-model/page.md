---
title: Understanding Regression Models in Machine Learning
description: Regression Models explained including linear logistic and regularized
  methods Evaluate performance with MSE and R squared Discover more inside
---



## Table of Contents

## What is a regression model in machine learning?

A regression model in machine learning is a type of algorithm used to predict a continuous outcome variable based on one or more predictor variables. Imagine you want to predict the price of a house based on its size, location, and age. A regression model can help you do that by finding a mathematical equation that best describes the relationship between these factors and the house price. This equation can then be used to make predictions for new houses based on their characteristics.

There are different types of regression models, but one of the simplest and most commonly used is linear regression. In linear regression, the relationship between the predictor variables and the outcome variable is modeled as a straight line. The equation for a simple linear regression with one predictor variable can be written as $$y = mx + b$$, where $$y$$ is the outcome variable, $$x$$ is the predictor variable, $$m$$ is the slope of the line, and $$b$$ is the y-intercept. The goal of the algorithm is to find the best values for $$m$$ and $$b$$ that minimize the difference between the predicted and actual values of $$y$$. This process involves fitting the model to a set of training data and then using it to make predictions on new data.

## What are the main types of regression models?

Regression models come in different types, each suited for different kinds of data and prediction tasks. The most basic type is linear regression, which assumes a straight-line relationship between the predictor variables and the outcome variable. In simple linear regression, the equation is $$y = mx + b$$, where $$y$$ is the outcome, $$x$$ is the predictor, $$m$$ is the slope, and $$b$$ is the y-intercept. Multiple linear regression extends this to more than one predictor variable, allowing for a more complex model that can capture the effects of multiple factors on the outcome.

Another common type is polynomial regression, which is used when the relationship between the predictors and the outcome is not linear but can be better described by a curve. The equation for polynomial regression can be written as $$y = a_n x^n + a_{n-1} x^{n-1} + ... + a_1 x + a_0$$, where the coefficients $$a_n$$ to $$a_0$$ are determined by the model. Logistic regression is used when the outcome variable is categorical, often binary (like yes/no or 0/1). It uses a logistic function to model the probability of the outcome, which is useful in fields like medicine for predicting the likelihood of a disease based on various risk factors.

Lastly, there are more advanced types like ridge regression and lasso regression, which are used when dealing with multicollinearity or when you want to prevent overfitting by adding a penalty to the regression model. Ridge regression adds a penalty equal to the square of the magnitude of the coefficients, while lasso regression adds a penalty equal to the absolute value of the magnitude of the coefficients. These methods help in selecting important variables and improving the model's performance on new data.

## How does linear regression work?

Linear regression is a way to predict a number by looking at other numbers. Imagine you want to guess how much a house will cost based on its size. Linear regression finds a straight line that best fits the data points of house sizes and their prices. This line can then be used to predict the price of a new house by just looking at its size. The equation for this line is $$y = mx + b$$, where $$y$$ is the price, $$x$$ is the size, $$m$$ is how steep the line is, and $$b$$ is where the line starts on the y-axis. The goal is to find the best $$m$$ and $$b$$ that make the line as close as possible to all the data points.

To find the best $$m$$ and $$b$$, linear regression uses a method called "least squares." This method calculates the difference between the actual house prices and the prices predicted by the line, squares these differences, and then adds them up. The best line is the one that makes this total as small as possible. Once the best line is found, it can be used to predict the price of a new house. For example, if the best line is $$y = 100x + 50000$$, and a new house has a size of 1500 square feet, the predicted price would be $$100 \times 1500 + 50000 = 200000$$ dollars.

## What is the difference between simple and multiple linear regression?

Simple linear regression is used when you want to predict a number based on just one other number. Imagine you're trying to guess how much a house will cost based on its size. Simple linear regression finds a straight line that best fits the data points of house sizes and their prices. The equation for this line is $$y = mx + b$$, where $$y$$ is the price, $$x$$ is the size, $$m$$ is how steep the line is, and $$b$$ is where the line starts on the y-axis. The goal is to find the best $$m$$ and $$b$$ that make the line as close as possible to all the data points.

Multiple linear regression is used when you want to predict a number based on more than one other number. For example, you might want to predict the price of a house based on its size, the number of bedrooms, and how old it is. Multiple linear regression finds a straight line in a higher-dimensional space that best fits the data points. The equation for multiple linear regression with three predictors could be written as $$y = m_1x_1 + m_2x_2 + m_3x_3 + b$$, where $$y$$ is the price, $$x_1$$ is the size, $$x_2$$ is the number of bedrooms, $$x_3$$ is the age, $$m_1, m_2, m_3$$ are how much each predictor affects the price, and $$b$$ is the starting point. The goal is to find the best values for $$m_1, m_2, m_3$$ and $$b$$ that make the line as close as possible to all the data points.

## What are the key assumptions of linear regression?

Linear regression makes some guesses about the data to work well. One guess is that the relationship between the numbers you're using to predict and the number you want to predict is a straight line. This means if you plot the data, it should look like it could be drawn with a ruler. Another guess is that the data points are spread out evenly around the line, not bunched up on one side. This is called homoscedasticity. If the data points are all over the place, the line won't be a good guess.

Another important guess is that the numbers you're using to predict are not too closely related to each other. This is called no multicollinearity. If they are too similar, it's hard to tell which one is really affecting the number you want to predict. Also, linear regression assumes that the errors, or the differences between the actual numbers and the numbers the line predicts, are normally distributed. This means if you made a bell curve of these errors, it would look like a normal bell shape. If these guesses are not true, the line might not be a good guess for new data.

Lastly, linear regression assumes that the errors are independent of each other. This means that knowing the error for one data point doesn't help you guess the error for another data point. If the errors are related, like if they go up and down together, the line might not work well for new data. These guesses help make sure the line is a good guess for the data and can be used to predict new numbers.

## How do you evaluate the performance of a regression model?

To evaluate how well a regression model works, you look at how close its predictions are to the actual numbers. One common way to do this is by using the Mean Squared Error (MSE). The MSE is calculated by taking the difference between each predicted number and the actual number, squaring these differences, and then finding the average of all these squared differences. The formula for MSE is $$ \text{MSE} = \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2 $$, where $$ y_i $$ is the actual number, $$ \hat{y}_i $$ is the predicted number, and $$ n $$ is the total number of data points. A smaller MSE means the model's predictions are closer to the actual numbers, so the model is doing a better job.

Another way to evaluate a regression model is by looking at the R-squared value. R-squared tells you how much of the change in the numbers you're trying to predict can be explained by the model. It's a number between 0 and 1, where 1 means the model explains all the change, and 0 means it explains none of it. The formula for R-squared is $$ R^2 = 1 - \frac{\sum_{i=1}^{n} (y_i - \hat{y}_i)^2}{\sum_{i=1}^{n} (y_i - \bar{y})^2} $$, where $$ \bar{y} $$ is the average of the actual numbers. A higher R-squared means the model is better at explaining the data. Both MSE and R-squared help you understand how well your regression model is working and whether it's a good guess for new data.

## What is polynomial regression and when is it used?

Polynomial regression is a type of regression model used when the relationship between the numbers you're using to predict and the number you want to predict is not a straight line but a curve. Imagine you're trying to guess how much a house will cost based on its size, but the prices don't go up in a straight line. Instead, they might go up slowly at first and then faster as the house gets bigger. Polynomial regression can find a curved line that fits this data better than a straight line. The equation for polynomial regression can be written as $$y = a_n x^n + a_{n-1} x^{n-1} + ... + a_1 x + a_0$$, where $$a_n$$ to $$a_0$$ are numbers the model figures out, and $$n$$ is how curvy the line is.

Polynomial regression is used when the straight line of simple or multiple linear regression doesn't fit the data well. For example, if you're looking at how the speed of a car affects how far it can go on a tank of gas, you might find that the relationship isn't a straight line. At low speeds, the car might go further, but as the speed goes up, the distance might start to drop off more quickly. Polynomial regression can capture this curve, making better guesses about how far the car will go at different speeds. By using a curved line instead of a straight one, polynomial regression can give more accurate predictions for data that doesn't follow a linear pattern.

## How does regularization help in regression models?

Regularization is like adding a little rule to regression models to stop them from getting too complicated. Imagine you're trying to guess how much a house will cost based on lots of different things about it, like size, age, and location. Without regularization, the model might start paying too much attention to tiny details that don't really matter, making it fit the training data perfectly but not work well for new houses. Regularization helps by adding a penalty to the model, making it simpler and better at guessing prices for new houses.

There are two main types of regularization: ridge and lasso. Ridge regularization adds a penalty to the model that's based on the square of the size of the numbers used to make guesses. This is called the L2 penalty, and it's written as $$ \text{Ridge Penalty} = \lambda \sum_{i=1}^{p} \beta_i^2 $$, where $$ \lambda $$ is how strong the penalty is, and $$ \beta_i $$ are the numbers the model uses. Lasso regularization, on the other hand, adds a penalty based on the absolute size of these numbers, called the L1 penalty, and it's written as $$ \text{Lasso Penalty} = \lambda \sum_{i=1}^{p} |\beta_i| $$. Lasso can even make some of these numbers zero, which means the model ignores some of the things about the house that don't help with guessing the price. Both types help make the model simpler and better at working with new data.

## What are some advanced regression techniques like ridge, lasso, and elastic net?

Ridge, lasso, and elastic net are advanced ways to make regression models better by adding a little rule to stop them from getting too complicated. Ridge regularization adds a penalty to the model that's based on the square of the size of the numbers used to make guesses. This is called the L2 penalty, and it's written as $$ \text{Ridge Penalty} = \lambda \sum_{i=1}^{p} \beta_i^2 $$, where $$ \lambda $$ is how strong the penalty is, and $$ \beta_i $$ are the numbers the model uses. This helps the model focus on the most important things and not get too caught up in tiny details. Lasso regularization, on the other hand, adds a penalty based on the absolute size of these numbers, called the L1 penalty, and it's written as $$ \text{Lasso Penalty} = \lambda \sum_{i=1}^{p} |\beta_i| $$. Lasso can even make some of these numbers zero, which means the model can ignore things that don't help with guessing the outcome.

Elastic net is a mix of ridge and lasso. It uses both the L1 and L2 penalties to make the model simpler and better at working with new data. The formula for elastic net is $$ \text{Elastic Net Penalty} = \lambda \left( \alpha \sum_{i=1}^{p} |\beta_i| + (1 - \alpha) \sum_{i=1}^{p} \beta_i^2 \right) $$, where $$ \alpha $$ is a number between 0 and 1 that decides how much of each penalty to use. If $$ \alpha $$ is 1, elastic net is just like lasso, and if it's 0, it's just like ridge. By using both penalties, elastic net can help the model focus on the most important things and also make some of the less important things zero, which can be really helpful when you have a lot of things to consider in your model.

## How do you handle multicollinearity in regression models?

Multicollinearity happens when the numbers you use to predict something in a regression model are too closely related to each other. Imagine you're trying to guess how much a house will cost based on its size and the number of rooms. If the size and the number of rooms are always similar, it's hard for the model to tell which one is really affecting the price. This can make the model's guesses less accurate and harder to understand. To deal with multicollinearity, you can remove some of the closely related numbers or combine them into one new number that captures what they have in common.

One way to handle multicollinearity is by using regularization techniques like ridge or lasso regression. Ridge regression adds a penalty to the model that's based on the square of the size of the numbers used to make guesses. This is called the L2 penalty, and it's written as $$ \text{Ridge Penalty} = \lambda \sum_{i=1}^{p} \beta_i^2 $$, where $$ \lambda $$ is how strong the penalty is, and $$ \beta_i $$ are the numbers the model uses. Lasso regression adds a penalty based on the absolute size of these numbers, called the L1 penalty, and it's written as $$ \text{Lasso Penalty} = \lambda \sum_{i=1}^{p} |\beta_i| $$. Lasso can even make some of these numbers zero, which means the model can ignore some of the closely related numbers. Both methods help the model focus on the most important things and make its guesses better for new data.

## What are non-linear regression models and how do they differ from linear models?

Non-linear regression models are used when the relationship between the numbers you're using to predict and the number you want to predict isn't a straight line. Imagine you're trying to guess how much a house will cost based on its size, but the prices don't go up in a straight line. Instead, they might go up slowly at first and then faster as the house gets bigger. Non-linear regression can find a curved line that fits this data better than a straight line. The equation for a non-linear model could be something like $$y = a e^{bx} + c$$, where $$a, b, c$$ are numbers the model figures out, and $$e$$ is a special number used in math. This type of model can capture the curve in the data, making better guesses about how much the house will cost.

Linear regression models, on the other hand, assume that the relationship between the predictors and the outcome is a straight line. If you plot the data, it should look like it could be drawn with a ruler. The equation for a simple linear regression is $$y = mx + b$$, where $$y$$ is the outcome, $$x$$ is the predictor, $$m$$ is how steep the line is, and $$b$$ is where the line starts on the y-axis. Linear models are simpler and easier to understand, but they can't capture the curves in the data that non-linear models can. If the data doesn't follow a straight line, a linear model might not be a good guess for new data, while a non-linear model can be more accurate by fitting a curve to the data.

## How can you use regression models for time series forecasting?

Regression models can be used for time series forecasting by treating time as one of the predictor variables. Imagine you want to guess how many ice creams will be sold each day based on the temperature and the day of the week. You can use a regression model where the number of ice creams sold is the outcome, and the temperature and the day of the week are the predictors. The model will find a line or a curve that best fits the data, and you can use this to predict how many ice creams will be sold on a new day based on the temperature and the day of the week. The equation for a simple linear regression could be $$y = mx + b$$, where $$y$$ is the number of ice creams sold, $$x$$ is the temperature, $$m$$ is how much the temperature affects sales, and $$b$$ is the starting point.

For more complex time series data, you might need to use non-linear regression models or add more predictors like the month or the year. These models can capture the ups and downs in the data over time, making better guesses about future sales. For example, if ice cream sales go up in the summer and down in the winter, a non-linear model can fit a curve to this pattern. The equation for a non-linear model could be something like $$y = a e^{bx} + c$$, where $$a, b, c$$ are numbers the model figures out, and $$e$$ is a special number used in math. By using these models, you can make more accurate predictions about how many ice creams will be sold in the future based on past data.

## References & Further Reading

[1]: James, G., Witten, D., Hastie, T., & Tibshirani, R. (2013). ["An Introduction to Statistical Learning: with Applications in R"](https://link.springer.com/book/10.1007/978-1-0716-1418-1). Springer.

[2]: Tibshirani, R. (1996). ["Regression Shrinkage and Selection via the Lasso."](https://webdoc.agsci.colostate.edu/koontz/arec-econ535/papers/Tibshirani%20(JRSS-B%201996).pdf) Journal of the Royal Statistical Society: Series B (Methodological), 58(1), 267-288.

[3]: Hoerl, A. E., & Kennard, R. W. (1970). ["Ridge Regression: Biased Estimation for Nonorthogonal Problems."](https://www.jstor.org/stable/1267351) Technometrics, 12(1), 55-67.

[4]: Bishop, C. M. (2006). ["Pattern Recognition and Machine Learning."](https://link.springer.com/book/9780387310732) Springer.

[5]: Montgomery, D. C., Peck, E. A., & Vining, G. G. (2012). ["Introduction to Linear Regression Analysis."](https://archive.org/download/econometrics_books/Intro.%20to%20Linear%20Regression%20Analysis%20-%20D.%20C.%20Montgomery%2C%20E.%20A.%20Peck.pdf) Wiley.

[6]: Gelman, A., & Hill, J. (2006). ["Data Analysis Using Regression and Multilevel/Hierarchical Models."](https://www.cambridge.org/highereducation/books/data-analysis-using-regression-and-multilevel-hierarchical-models/32A29531C7FD730C3A68951A17C9D983) Cambridge University Press.

[7]: Seber, G. A. F., & Lee, A. J. (2012). ["Linear Regression Analysis."](https://onlinelibrary.wiley.com/doi/book/10.1002/9780471722199) Wiley.