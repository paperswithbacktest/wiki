---
category: quant_concept
description: L1 Loss measures model error by averaging absolute differences, reducing
  outlier impact and enhancing feature selection Discover more inside
title: Understanding L1 Loss in Machine Learning Regression
---

![Image](images/1.png)

## Table of Contents

## What is L1 Loss in machine learning?

L1 Loss, also known as Least Absolute Deviations (LAD) or Mean Absolute Error (MAE), is a way to measure how wrong a machine learning model's predictions are. It does this by looking at the absolute difference between what the model predicts and the actual correct answer. Imagine you guessed that a book weighs 2 pounds, but it actually weighs 3 pounds. The L1 Loss would be the absolute difference, which is 1 pound. This method is useful because it treats all errors the same, no matter how big or small they are.

In math, L1 Loss can be written as $$L_1 = \frac{1}{n} \sum_{i=1}^{n} |y_i - \hat{y}_i|$$, where $$n$$ is the number of predictions, $$y_i$$ is the actual value, and $$\hat{y}_i$$ is the predicted value. This formula shows that we add up all the absolute differences and then divide by the total number of predictions to get an average error. L1 Loss is often used when you want your model to be less sensitive to outliers, because it doesn't square the errors like L2 Loss does, which can make big errors even bigger.

## How does L1 Loss differ from other loss functions like L2 Loss?

L1 Loss and L2 Loss are two different ways to measure how wrong a machine learning model's predictions are. L1 Loss, also called Mean Absolute Error (MAE), looks at the absolute difference between the predicted value and the actual value. For example, if you predicted a temperature of 20 degrees but it was actually 25 degrees, the L1 Loss would be 5 degrees. This is calculated using the formula $$L_1 = \frac{1}{n} \sum_{i=1}^{n} |y_i - \hat{y}_i|$$, where $$n$$ is the number of predictions, $$y_i$$ is the actual value, and $$\hat{y}_i$$ is the predicted value. L1 Loss treats all errors the same, no matter how big or small they are, which makes it less sensitive to outliers.

On the other hand, L2 Loss, also known as Mean Squared Error (MSE), squares the differences between the predicted and actual values before summing them up. Using the same temperature example, if you predicted 20 degrees but it was actually 25 degrees, the L2 Loss would be $$5^2 = 25$$ degrees squared. The formula for L2 Loss is $$L_2 = \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2$$. Because L2 Loss squares the errors, it makes bigger errors even bigger, which can be useful when you want to penalize larger mistakes more heavily. This sensitivity to outliers can be both an advantage and a disadvantage, depending on the specific needs of your model.

## Why is L1 Loss also known as Least Absolute Deviations (LAD)?

L1 Loss is also known as Least Absolute Deviations (LAD) because it measures the error between predictions and actual values by taking the absolute value of their differences. This means that whether a prediction is too high or too low, the error is counted the same way. For example, if you predicted a number to be 10 but it was actually 15, the L1 Loss would be 5. If you predicted 20 instead, the L1 Loss would still be 5. This method is called "Least Absolute Deviations" because it tries to make the total of these absolute differences as small as possible.

In math, L1 Loss can be written as $$L_1 = \frac{1}{n} \sum_{i=1}^{n} |y_i - \hat{y}_i|$$, where $$n$$ is the number of predictions, $$y_i$$ is the actual value, and $$\hat{y}_i$$ is the predicted value. This formula shows that we add up all the absolute differences and then divide by the total number of predictions to get an average error. Because L1 Loss focuses on minimizing the sum of these absolute errors, it's a straightforward way to measure how well a model is doing without being overly affected by very large errors, which is why it's called Least Absolute Deviations.

## In what scenarios is L1 Loss particularly useful?

L1 Loss, or Mean Absolute Error (MAE), is especially useful in situations where you want your model to be less sensitive to big mistakes, called outliers. Imagine you're predicting house prices, and most houses are around $200,000, but one house is $2,000,000. If you use L1 Loss, a wrong guess on the expensive house won't mess up your model as much as it would with other methods. This is because L1 Loss uses the absolute difference, so a big mistake is treated the same as a small one, just with a bigger number.

Another good time to use L1 Loss is when you want to keep things simple and easy to understand. The formula for L1 Loss is $$L_1 = \frac{1}{n} \sum_{i=1}^{n} |y_i - \hat{y}_i|$$, which means you just add up all the absolute differences between what you guessed and what's actually true, then divide by how many guesses you made. This makes it easier to explain to others and to use in models where you want to see a clear picture of how well you're doing without getting lost in complicated math.

## How do you calculate L1 Loss for a given set of predictions and actual values?

To calculate L1 Loss for a set of predictions and actual values, you need to find the absolute difference between each prediction and its corresponding actual value. Then, you add up all these absolute differences and divide by the total number of predictions. This gives you the average absolute error, which is the L1 Loss. For example, if you predicted temperatures of 20, 22, and 24 degrees, but the actual temperatures were 21, 23, and 25 degrees, you would calculate the absolute differences as 1, 1, and 1. Adding these up gives you 3, and dividing by the number of predictions (3) gives you an L1 Loss of 1 degree.

In math, the formula for L1 Loss is $$L_1 = \frac{1}{n} \sum_{i=1}^{n} |y_i - \hat{y}_i|$$, where $$n$$ is the number of predictions, $$y_i$$ is the actual value, and $$\hat{y}_i$$ is the predicted value. This formula shows that you sum up all the absolute differences between the actual and predicted values and then divide by the total number of predictions to get the average error. If you want to calculate this in a programming language like Python, you can use a simple code block like this:

```python
import numpy as np

# Example data
actual_values = [21, 23, 25]
predicted_values = [20, 22, 24]

# Calculate L1 Loss
l1_loss = np.mean(np.abs(np.array(actual_values) - np.array(predicted_values)))
print("L1 Loss:", l1_loss)
```

This code calculates the L1 Loss by finding the mean of the absolute differences between the actual and predicted values, giving you the same result as the manual calculation.

## What are the advantages of using L1 Loss in regression problems?

L1 Loss, also known as Mean Absolute Error (MAE), is really helpful in regression problems because it's not too affected by big mistakes. Imagine you're guessing the weights of a bunch of apples, and one apple is much heavier than the others. If you make a big mistake on that heavy apple, it won't mess up your overall guess as much as it would with other methods. L1 Loss does this by looking at the absolute difference between your guess and the real weight, so a big mistake is treated the same as a small one, just with a bigger number. This makes it easier to keep your model working well even when there are a few big errors.

Another good thing about L1 Loss is that it's easy to understand and use. The way you calculate it is simple: you just find the absolute difference between each guess and the real value, add all those differences up, and then divide by how many guesses you made. This is shown in the formula $$L_1 = \frac{1}{n} \sum_{i=1}^{n} |y_i - \hat{y}_i|$$, where $$n$$ is the number of guesses, $$y_i$$ is the real value, and $$\hat{y}_i$$ is your guess. Because it's easy to explain and understand, L1 Loss is great for models where you want to see a clear picture of how well you're doing without getting lost in complicated math.

## Can L1 Loss lead to sparse models? If so, how?

L1 Loss can lead to sparse models when it's used as a regularization technique, often called L1 regularization or Lasso. In simple terms, a sparse model means that some of the model's parameters, like the weights in a regression model, become zero. This happens because L1 Loss adds the absolute values of the weights to the loss function, which encourages the model to shrink some weights all the way to zero. The formula for L1 regularization is $$L = L_1 + \alpha \sum_{j=1}^{p} |w_j|$$, where $$L_1$$ is the L1 Loss, $$\alpha$$ is a hyperparameter that controls the strength of the regularization, and $$w_j$$ are the model's weights. By making some weights zero, the model becomes simpler and easier to interpret, as it focuses only on the most important features.

When L1 Loss is used for regularization, it helps in feature selection because it can effectively remove less important features from the model. This is particularly useful in datasets with many features, where it can be hard to tell which ones are really important. By setting some weights to zero, L1 regularization helps to avoid overfitting by reducing the model's complexity. This makes the model more generalizable to new data, as it's less likely to be influenced by noise or irrelevant features in the training data.

## How does L1 Loss affect the training process of a neural network?

When you use L1 Loss to train a [neural network](/wiki/neural-network), it affects the training process by making the network focus on reducing the average absolute error between its predictions and the actual values. This means the network tries to minimize the sum of the absolute differences between what it guesses and what's true, divided by the total number of guesses. The formula for L1 Loss is $$L_1 = \frac{1}{n} \sum_{i=1}^{n} |y_i - \hat{y}_i|$$, where $$n$$ is the number of predictions, $$y_i$$ is the actual value, and $$\hat{y}_i$$ is the predicted value. Because L1 Loss treats all errors the same, it's less affected by big mistakes, which can make the training process more stable and less influenced by outliers.

Using L1 Loss can also lead to sparse models if it's used as a regularization technique. This means some of the weights in the neural network can become zero, making the model simpler and easier to understand. The formula for L1 regularization is $$L = L_1 + \alpha \sum_{j=1}^{p} |w_j|$$, where $$L_1$$ is the L1 Loss, $$\alpha$$ is a hyperparameter that controls the strength of the regularization, and $$w_j$$ are the model's weights. By setting some weights to zero, the network focuses on the most important features, which can help prevent overfitting and make the model more generalizable to new data.

## What are the potential drawbacks of using L1 Loss?

Using L1 Loss can have some downsides. One big problem is that it can be hard to work with when you're trying to make your model better. L1 Loss isn't smooth because it uses the absolute value, which means it has sharp corners. This can make it tricky for the computer to find the best way to improve the model because it has to deal with these sudden changes. Imagine trying to roll a ball down a road with lots of bumps; it's hard to keep the ball moving smoothly. The formula for L1 Loss is $$L_1 = \frac{1}{n} \sum_{i=1}^{n} |y_i - \hat{y}_i|$$, and the sharp corners come from the absolute value part, $$|y_i - \hat{y}_i|$$.

Another issue with L1 Loss is that it might not be the best choice if you really care about big mistakes. Because L1 Loss treats all errors the same, whether they're big or small, it doesn't pay more attention to really big errors. This can be a problem if you're working on something where big mistakes are much worse than small ones. For example, if you're predicting how much medicine someone needs, a big mistake could be dangerous, and you'd want your model to try harder to avoid those big errors. In those cases, using a different type of loss, like L2 Loss, might be better because it squares the errors and makes big mistakes count more.

## How can L1 Loss be implemented in popular machine learning libraries like TensorFlow or PyTorch?

In TensorFlow, you can implement L1 Loss easily using the `tf.keras.losses.MeanAbsoluteError` function. This function calculates the average absolute difference between the predicted values and the actual values. To use it, you just need to create an instance of the `MeanAbsoluteError` class and then call it with your predictions and true values. Here's how you can do it in a simple code block:

```python
import tensorflow as tf

# Example data
y_true = tf.constant([1, 2, 3])
y_pred = tf.constant([1.2, 1.9, 3.1])

# Calculate L1 Loss
mae = tf.keras.losses.MeanAbsoluteError()
l1_loss = mae(y_true, y_pred)
print("L1 Loss:", l1_loss.numpy())
```

In PyTorch, you can implement L1 Loss using the `torch.nn.L1Loss` class. This class also calculates the average absolute difference between the predicted and actual values. You create an instance of `L1Loss` and then call it with your predictions and true values. Here's a simple example of how to do it in PyTorch:

```python
import torch
import torch.nn as nn

# Example data
y_true = torch.tensor([1.0, 2.0, 3.0])
y_pred = torch.tensor([1.2, 1.9, 3.1])

# Calculate L1 Loss
l1_loss = nn.L1Loss()
loss = l1_loss(y_pred, y_true)
print("L1 Loss:", loss.item())
```

Both of these examples show how you can use L1 Loss, which is calculated using the formula $$L_1 = \frac{1}{n} \sum_{i=1}^{n} |y_i - \hat{y}_i|$$, where $$n$$ is the number of predictions, $$y_i$$ is the actual value, and $$\hat{y}_i$$ is the predicted value. This formula helps you understand that L1 Loss is just the average of the absolute differences between your guesses and the real values.

## What are some advanced techniques for optimizing models using L1 Loss?

One advanced technique for optimizing models using L1 Loss is to use it as a regularization method, often called Lasso regularization. This means you add the absolute values of the model's weights to the L1 Loss, which encourages the model to shrink some weights all the way to zero. The formula for this is $$L = L_1 + \alpha \sum_{j=1}^{p} |w_j|$$, where $$L_1$$ is the L1 Loss, $$\alpha$$ is a hyperparameter that controls how strong the regularization is, and $$w_j$$ are the model's weights. By making some weights zero, the model becomes simpler and easier to understand, focusing only on the most important features. This helps prevent overfitting and can make the model work better on new data.

Another technique is to combine L1 Loss with other loss functions to create a hybrid approach. For example, you might use L1 Loss for the main part of your model's training but also use L2 Loss to pay more attention to big mistakes. This can be done by using a weighted sum of the two losses, where you decide how much each loss affects the overall error. In code, this might look like:

```python
import tensorflow as tf

y_true = tf.constant([1, 2, 3])
y_pred = tf.constant([1.2, 1.9, 3.1])

# Calculate L1 Loss
mae = tf.keras.losses.MeanAbsoluteError()
l1_loss = mae(y_true, y_pred)

# Calculate L2 Loss
mse = tf.keras.losses.MeanSquaredError()
l2_loss = mse(y_true, y_pred)

# Combine L1 and L2 Loss with a weight
alpha = 0.5  # You can adjust this
combined_loss = alpha * l1_loss + (1 - alpha) * l2_loss
print("Combined Loss:", combined_loss.numpy())
```

This approach can help balance the benefits of L1 Loss, which is less affected by outliers, with the benefits of L2 Loss, which pays more attention to big mistakes. By tweaking the weights, you can find the best mix for your specific problem.

## How does L1 Loss compare to other robust loss functions in handling outliers?

L1 Loss, or Mean Absolute Error (MAE), is good at dealing with outliers because it looks at the absolute difference between predictions and actual values. This means that whether a mistake is big or small, it counts the same way. For example, if you guessed a number was 10 but it was really 20, the L1 Loss would be 10. If you guessed 12 instead, the L1 Loss would be 8. This makes L1 Loss less affected by big mistakes, which is helpful when you have some data points that are very different from the rest. The formula for L1 Loss is $$L_1 = \frac{1}{n} \sum_{i=1}^{n} |y_i - \hat{y}_i|$$, where $$n$$ is the number of predictions, $$y_i$$ is the actual value, and $$\hat{y}_i$$ is the predicted value.

Other robust loss functions, like the Huber Loss, also try to handle outliers well but in different ways. Huber Loss is a mix of L1 and L2 Loss. It uses L2 Loss for small errors, which squares the differences, and L1 Loss for big errors, which uses the absolute value. This means it can pay more attention to small mistakes while still being less affected by big ones. The formula for Huber Loss is more complicated, but it's designed to be a good middle ground between L1 and L2 Loss. In practice, choosing between L1 Loss and other robust loss functions depends on how much you care about big mistakes and how much you want your model to be simple and easy to understand.

## References & Further Reading

[1]: Friedman, J. H., Hastie, T., & Tibshirani, R. (2001). ["The Elements of Statistical Learning"](https://link.springer.com/book/10.1007/978-0-387-84858-7). Springer Series in Statistics.

[2]: Tibshirani, R. (1996). ["Regression Shrinkage and Selection via the Lasso."](https://webdoc.agsci.colostate.edu/koontz/arec-econ535/papers/Tibshirani%20(JRSS-B%201996).pdf) Journal of the Royal Statistical Society: Series B (Methodological), 267-288.

[3]: Goodfellow, I., Bengio, Y., & Courville, A. (2016). ["Deep Learning"](https://www.deeplearningbook.org/) MIT Press.

[4]: Huber, P. J. (1964). ["Robust Estimation of a Location Parameter."](https://projecteuclid.org/journals/annals-of-mathematical-statistics/volume-35/issue-1/Robust-Estimation-of-a-Location-Parameter/10.1214/aoms/1177703732.full) The Annals of Mathematical Statistics, 35(1), 73-101.

[5]: Murphy, K. P. (2012). ["Machine Learning: A Probabilistic Perspective"](https://www.cs.ubc.ca/~murphyk/MLbook/pml-toc-1may12.pdf) MIT Press.