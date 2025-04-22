---
title: Understanding Linear Regression Assumptions and Limitations
description: Linear regression assumptions ensure reliable predictions by validating
  linearity homoscedasticity independence and normality Discover more inside
---


![Image](images/1.png)

## Table of Contents

## What is linear regression?

Linear regression is a way to find out how one thing affects another. Imagine you want to know how the number of hours you study affects your test scores. Linear regression helps you draw a straight line through your data points to show this relationship. The line shows the best guess of how much your test score will go up for every extra hour you study.

This method uses math to find the line that comes closest to all the points on your graph. The line is described by a formula, usually written as y = mx + b, where 'y' is what you're trying to predict (like test scores), 'x' is what you're using to predict it (like study hours), 'm' is the slope of the line (how much the test score changes with each hour), and 'b' is where the line starts on the y-axis (the score you'd get with zero study hours). Linear regression is used a lot because it's simple and works well for many kinds of data.

## What are the basic assumptions of linear regression?

Linear regression works best when certain things are true about your data. One key assumption is that the relationship between the thing you're trying to predict (like test scores) and the thing you're using to predict it (like study hours) is a straight line. If the relationship is curved or zigzag, linear regression won't be the best choice. Another important assumption is that the errors, or the difference between the actual data points and the line you draw, are spread out evenly. This means that the mistakes you make in guessing the test scores should be random and not follow any pattern.

Another assumption is that the errors are normally distributed. This means that if you made a bell-shaped curve of all your errors, it would look normal, with most errors being small and fewer big errors on both sides. Also, the errors for different data points should not be connected. For example, the error you make guessing one student's test score should not affect the error you make guessing another student's score. Lastly, the thing you're using to predict (like study hours) should be measured without any errors, and all the important factors that affect what you're trying to predict should be included in your model. If you miss an important [factor](/wiki/factor-investing), like the amount of sleep students get, your predictions might not be very accurate.

## How does the assumption of linearity affect the model's performance?

The assumption of linearity means that the relationship between what you're trying to predict and what you're using to predict it should be a straight line. If this isn't true, your model might not work well. For example, if studying more hours leads to better test scores, but only up to a point, and then more studying doesn't help anymore, a straight line won't fit the data well. This can make your predictions less accurate because the line won't match the real pattern of the data.

When the relationship isn't linear, using a linear regression model can lead to big mistakes in your predictions. Imagine if the real relationship between study hours and test scores is a curve. A straight line might go through some of the data points, but it won't capture the curve. This means that for some values of study hours, the line will predict test scores that are too high or too low. So, checking if the relationship is really linear before using linear regression is important to make sure your model works well.

## What is the importance of the independence of errors assumption?

The independence of errors assumption means that the mistakes you make in guessing one data point should not affect the mistakes you make in guessing another data point. Imagine you're trying to predict test scores based on study hours. If the error you make in guessing one student's score affects the error you make in guessing another student's score, then the errors are not independent. This can happen if students are grouped in some way, like if they all study together or if they're from the same class. If errors are not independent, it can mess up your predictions and make your model less accurate.

When errors are not independent, it can lead to a problem called autocorrelation. This means that the errors are related to each other in a way that follows a pattern. For example, if you're predicting sales over time, and the errors for one month affect the errors for the next month, your model might think there's a trend when there isn't one. This can make your model think it's doing better than it really is, because it's just following the pattern in the errors instead of the real pattern in the data. So, making sure the errors are independent is important for making sure your linear regression model is reliable and gives you good predictions.

## How can we check for homoscedasticity in linear regression?

Homoscedasticity means that the errors, or the difference between what you predict and what actually happens, should be spread out evenly across all values of what you're using to predict. Imagine you're guessing test scores based on study hours. If the errors are homoscedastic, the mistakes you make should be about the same, no matter how many hours someone studies. If the errors get bigger or smaller as study hours change, then you don't have homoscedasticity, and this can make your predictions less reliable.

To check for homoscedasticity, you can make a scatter plot of the residuals, which are the errors, against the predicted values. If the points on the scatter plot are spread out evenly, and there's no clear pattern where the spread of the points gets wider or narrower, then you probably have homoscedasticity. Another way to check is by using a statistical test called the Breusch-Pagan test. If this test shows that the errors are not spread out evenly, then you might need to fix your model to make it work better.

## What are the consequences of violating the normality assumption?

The normality assumption means that the errors, or the differences between what you predict and what actually happens, should follow a normal distribution. This is like a bell-shaped curve where most errors are small and there are fewer big errors on both sides. If this assumption is not true, it can make your predictions less reliable. For example, if the errors are not normally distributed, the confidence intervals you use to guess how sure you are about your predictions might not be accurate. This means you might think you're more sure about your predictions than you really are.

Also, when the normality assumption is violated, some statistical tests you might use to check your model, like t-tests or F-tests, might not work properly. These tests help you understand if the things you're using to predict (like study hours) really affect what you're trying to predict (like test scores). If the errors are not normal, these tests might say things are important when they're not, or not important when they are. So, it's a good idea to check if your errors are normally distributed, maybe by making a histogram or using a test like the Shapiro-Wilk test, to make sure your model is giving you good information.

## How does multicollinearity impact linear regression models?

Multicollinearity happens when the things you're using to predict something are too closely related to each other. Imagine you're trying to guess how well students will do on a test based on how many hours they study and how many pages they read. If studying more hours always means reading more pages, these two things are closely related, and that's multicollinearity. When this happens, it can make it hard for your model to figure out which of these things is really helping you predict the test scores. It's like trying to separate the effects of two things that always happen together.

This can cause big problems in your model. For one, it can make the numbers (called coefficients) that tell you how much each thing affects the test scores seem weird or wrong. They might be too big or too small, or even have the wrong sign, like saying more studying makes test scores worse when it really helps. Also, it can make your model less reliable because small changes in your data can lead to big changes in your predictions. So, it's important to check for multicollinearity, maybe by looking at something called the Variance Inflation Factor (VIF), and if you find it, you might need to change your model to make it work better.

## What are some common methods to detect multicollinearity?

One way to check for multicollinearity is by looking at the correlation between the things you're using to predict something. If two of these things are very closely related, like if studying more hours always means reading more pages, you might have a problem. You can make a correlation matrix to see this. If you see numbers close to 1 or -1, it means those things are too similar, and you should think about changing your model.

Another way is to use something called the Variance Inflation Factor (VIF). This is a number that tells you how much the other things you're using to predict are making it hard to figure out the effect of one thing. If the VIF is too high, usually more than 5 or 10, it means you have multicollinearity. You can use special software to calculate the VIF and see if you need to fix your model.

Lastly, you can also look at how stable your model is. If small changes in your data make big changes in your predictions, it might be because of multicollinearity. This is called instability, and it's a sign that the things you're using to predict are too closely related. Checking for this can help you make your model better and more reliable.

## How can outliers affect the results of a linear regression?

Outliers are data points that are very different from the others. They can mess up a linear regression model a lot. Imagine you're trying to guess how much studying affects test scores. If one student studied a lot but got a really low score, that student's data would be an outlier. This outlier can pull the line that the model draws away from where it should be, making all the predictions less accurate. The line might end up too high or too low because it's trying to include the outlier, and that means the guesses for everyone else's test scores will be off.

It's a good idea to check for outliers before you finish your model. You can look at a scatter plot to see if there are any points that are far away from the others. If you find an outlier, you need to think about why it's there. Maybe there's a good reason for it, like the student was sick during the test, and you might decide to keep it in your model. Or maybe it's just a mistake, and you can take it out to make your model work better. Either way, knowing about outliers can help you make better guesses with your linear regression model.

## What are the limitations of linear regression when dealing with non-linear relationships?

Linear regression works best when the relationship between what you're trying to predict and what you're using to predict it is a straight line. But if the relationship is not a straight line, like if it's a curve or a zigzag, linear regression can have problems. Imagine you're trying to guess how much studying affects test scores, but the real pattern is that studying helps a lot at first, then not as much. A straight line won't fit this pattern well, so your guesses about test scores will be off.

When you use linear regression on data with a non-linear relationship, the line you draw will be wrong for a lot of the data points. This means your predictions will be less accurate. For example, if the real relationship is a curve, the straight line might be too high for some study hours and too low for others. To fix this, you might need to use a different kind of model that can handle curves or other shapes, like polynomial regression or a non-linear model.

## How can we address the limitations of linear regression in practice?

When the relationship between what you're trying to predict and what you're using to predict it isn't a straight line, you can try other kinds of models instead of linear regression. For example, if the relationship looks like a curve, you could use polynomial regression. This kind of model can fit curves by adding more terms to the equation, like x-squared or x-cubed. Another option is to use non-linear regression models, which can fit all sorts of shapes and patterns that linear regression can't handle. These models can give you better predictions when the real relationship is more complicated than a straight line.

Another way to deal with the limits of linear regression is to change your data before you use it. You can try transforming your data, like taking the log or the square root of your numbers. This can turn a curved relationship into a straight one, so linear regression can work better. Also, if you think there might be more than one thing affecting what you're trying to predict, you can add those things to your model. This is called multiple regression, and it can help you get a more accurate picture of what's really going on. By trying different methods and checking which one works best, you can make your predictions more reliable even when the real world isn't a straight line.

## What advanced techniques can be used to overcome the limitations of traditional linear regression?

One advanced technique to overcome the limitations of traditional linear regression is using polynomial regression. This method lets you fit a curve to your data instead of just a straight line. Imagine you're trying to guess how much studying affects test scores, but the real pattern is that studying helps a lot at first and then not as much. A straight line won't fit this pattern well, but polynomial regression can. It adds extra terms to the equation, like x-squared or x-cubed, so it can bend and twist to match the curve of your data. This can make your predictions more accurate when the relationship isn't a straight line.

Another technique is to use non-linear regression models. These models can fit all sorts of shapes and patterns that linear regression can't handle. For example, if the relationship between studying and test scores is really complicated, like a zigzag or an S-shape, a non-linear model can capture that. These models use different math to find the best fit for your data, which can give you better predictions. You can also try transforming your data before using it in a model. For instance, taking the log or the square root of your numbers can turn a curved relationship into a straight one, so linear regression can work better. By trying different methods and checking which one works best, you can make your predictions more reliable even when the real world isn't a straight line.

## What is Linear Regression?

Linear regression is a fundamental statistical method employed to model the relationship between a dependent variable and one or more independent variables. This relationship is expressed in a linear form, meaning it assumes that changes in the independent variables result in proportional changes in the dependent variable. The basic equation of a simple linear regression can be represented as:

$$

Y = \beta_0 + \beta_1X + \epsilon 
$$

where $Y$ is the dependent variable, $X$ represents the independent variable, $\beta_0$ is the y-intercept, $\beta_1$ is the slope of the line, and $\epsilon$ is the error term signifying the difference between the observed and predicted values.

Linear regression extends to multiple independent variables through multiple linear regression, represented as:

$$

Y = \beta_0 + \beta_1X_1 + \beta_2X_2 + \ldots + \beta_nX_n + \epsilon 
$$

where each $X_i$ represents different independent variables affecting $Y$.

A crucial aspect of linear regression is the method used to estimate the coefficients or parameters ($\beta$ values). Ordinary Least Squares (OLS) is the most commonly used technique for this purpose. The principle of OLS is to minimize the sum of the squared differences between the observed values and those predicted by the linear model. This sum can be expressed as:

$$

\text{minimize} \quad \sum_{i=1}^{n} (Y_i - \hat{Y_i})^2 
$$

By minimizing this function, the OLS method provides the "best fit" line through the data points in the dataset.

The simplicity and interpretability of linear regression make it an attractive choice for modeling in various fields, including finance. However, its assumptions and limitations must be carefully considered to ensure model validity. Linear relationships are not always the best representation of complex real-world data, particularly in financial markets, which often exhibit non-linear patterns due to a multitude of factors.

## References & Further Reading

[1]: Bergstra, J., Bardenet, R., Bengio, Y., & Kégl, B. (2011). ["Algorithms for Hyper-Parameter Optimization."](https://papers.nips.cc/paper/4443-algorithms-for-hyper-parameter-optimization) Advances in Neural Information Processing Systems 24.

[2]: ["Advances in Financial Machine Learning"](https://www.amazon.com/Advances-Financial-Machine-Learning-Marcos/dp/1119482089) by Marcos Lopez de Prado

[3]: ["Evidence-Based Technical Analysis: Applying the Scientific Method and Statistical Inference to Trading Signals"](https://www.amazon.com/Evidence-Based-Technical-Analysis-Scientific-Statistical/dp/0470008741) by David Aronson

[4]: ["Machine Learning for Algorithmic Trading"](https://github.com/stefan-jansen/machine-learning-for-trading) by Stefan Jansen

[5]: ["Quantitative Trading: How to Build Your Own Algorithmic Trading Business"](https://books.google.com/books/about/Quantitative_Trading.html?id=j70yEAAAQBAJ) by Ernest P. Chan