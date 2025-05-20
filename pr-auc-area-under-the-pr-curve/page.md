---
category: quant_concept
description: PR AUC evaluation guides your model to balance precision and recall on
  imbalanced data for clearer performance insights. Discover more inside.
title: Understanding PR AUC Performance Metric in Machine Learning
---

## Table of Contents

## What is the PR AUC and why is it important in machine learning?

PR AUC stands for Precision-Recall Area Under the Curve. It's a way to measure how well a machine learning model can tell apart the things it's supposed to find from the things it's not supposed to find. Imagine you're looking for red apples in a pile of fruits. Precision is how many of the fruits you picked up are actually red apples, and recall is how many of the red apples in the pile you managed to pick up. The PR AUC combines these two measures over different thresholds and gives you one number that shows how good your model is at this task.

PR AUC is important in machine learning, especially when the data you're working with is unbalanced. This means there are a lot more of one type of thing than another. For example, if you're trying to find a rare disease in a large population, you want your model to be really good at spotting the few cases that exist. PR AUC helps you see how well your model does this job across different levels of strictness, or thresholds. A higher PR AUC means your model is better at balancing between finding all the cases (high recall) and making sure the cases it finds are actually correct (high precision).

## How does the PR AUC differ from the ROC AUC?

PR AUC and ROC AUC are both ways to measure how good a machine learning model is, but they focus on different things. PR AUC looks at precision and recall. Precision is about how many of the things your model says are correct actually are correct. Recall is about how many of the correct things your model finds. PR AUC is really helpful when you're dealing with data where one type of thing is much rarer than others. It shows how well your model can find these rare things while still being accurate.

ROC AUC, on the other hand, focuses on the true positive rate (sensitivity) and the false positive rate. It's about how well your model can tell the difference between the things it should find and the things it shouldn't. ROC AUC is good when you want to see how your model performs across all possible thresholds, but it can be less useful when your data is very unbalanced. In those cases, PR AUC can give you a better picture of how well your model is doing at finding the rare things you care about.

Both measures give you a number between 0 and 1, where 1 is perfect and 0 is the worst. The formulas for them are a bit different, but they both involve calculating areas under curves. For PR AUC, you're looking at the area under the precision-recall curve, and for ROC AUC, it's the area under the receiver operating characteristic curve.

## What are precision and recall, and how do they relate to the PR curve?

Precision and recall are two important measures used to see how well a [machine learning](/wiki/machine-learning) model is doing its job. Precision is about how many of the things the model says are correct actually are correct. Imagine you're looking for red apples in a pile of fruits. If you pick up 10 fruits and 8 of them are red apples, your precision is 80%. Recall, on the other hand, is about how many of the correct things the model finds. If there are 10 red apples in the pile and you pick up 8 of them, your recall is 80%. Both measures are important, but they focus on different aspects of the model's performance.

The PR curve, or precision-recall curve, shows how precision and recall change as you adjust the threshold of your model. The threshold is like a line that decides what the model says is a red apple and what it says isn't. As you move this line, you get different values for precision and recall. The PR curve plots these values, with recall on the x-axis and precision on the y-axis. The area under this curve, called the PR AUC, gives you a single number that shows how well your model is balancing precision and recall across all thresholds. A higher PR AUC means your model is doing a better job at finding the right things while keeping its guesses accurate.

## How is the PR curve constructed from a set of predictions?

To construct a PR curve from a set of predictions, you start by sorting the predictions by their confidence scores, from highest to lowest. For each prediction, you decide if it's a positive or negative example based on a threshold. As you move the threshold from high to low, you calculate the precision and recall at each point. Precision is the number of true positives divided by the total number of positives your model predicted, and recall is the number of true positives divided by the total number of actual positives in your data. You plot these values on a graph, with recall on the x-axis and precision on the y-axis.

As you lower the threshold, more predictions are classified as positive, which usually increases the recall but might decrease the precision. You keep track of these values and plot them to form the PR curve. The area under this curve, called the PR AUC, gives you a single number that summarizes how well your model balances precision and recall across all thresholds. A higher PR AUC means your model is better at finding the correct things while keeping its guesses accurate.

## What does a high PR AUC value indicate about a model's performance?

A high PR AUC value means that a model is doing a good job at finding the things it's supposed to find while also making sure its guesses are correct. Imagine you're looking for red apples in a pile of fruits. A high PR AUC means your model is good at [picking](/wiki/asset-class-picking) up most of the red apples (high recall) and also making sure that most of the fruits it picks up are actually red apples (high precision). This balance is important, especially when the thing you're looking for is rare, like finding a needle in a haystack.

The PR AUC looks at how well the model does this balancing act across different levels of strictness, or thresholds. A perfect model would have a PR AUC of 1, which means it finds all the right things and never makes a wrong guess. In real life, a high PR AUC, like 0.9 or above, shows that the model is very good at its job. It's a helpful number to know because it gives you a clear idea of how well your model works, especially when you're dealing with data where one thing is much rarer than others.

## How can you interpret the shape of the PR curve?

The shape of the PR curve tells you how well a model balances between finding the right things and making sure its guesses are correct. If the curve is high and stays close to the top right corner, it means the model is doing a great job. It's picking up most of the things it should find (high recall) and most of the things it picks up are correct (high precision). A curve that drops quickly shows the model might be good at finding things at first but gets less accurate as it tries to find more.

If the PR curve looks like a straight line from the top left to the bottom right, it means the model is just guessing randomly. The area under this curve, the PR AUC, would be low, showing the model isn't very good at its job. A model with a PR curve that stays high for a long time before dropping is better because it keeps a good balance of precision and recall over different levels of strictness.

## What are some common scenarios where PR AUC is more appropriate than ROC AUC?

PR AUC is more useful than ROC AUC when you're trying to find something that's rare in your data. Imagine you're looking for a few red apples in a big pile of fruits. You want your model to be really good at spotting those few red apples while not picking up too many other fruits by mistake. PR AUC helps you see how well your model does this job. It focuses on how many of the things your model says are correct actually are correct (precision) and how many of the correct things your model finds (recall). When the thing you're looking for is rare, PR AUC gives you a better idea of how well your model is working.

Another scenario where PR AUC is more appropriate is when the cost of false positives is high. For example, if you're trying to find a rare disease in a large population, you don't want your model to say too many healthy people have the disease. PR AUC is better at showing how well your model can balance finding the few sick people (high recall) while not labeling too many healthy people as sick (high precision). This makes PR AUC a better choice when the balance between precision and recall is really important.

## How do class imbalance issues affect the PR AUC?

Class imbalance happens when one type of thing in your data is much rarer than others. Imagine you're looking for red apples in a big pile of fruits, but there are only a few red apples. When you use PR AUC to see how well your model is doing, it helps you focus on how good the model is at finding those few red apples while not picking up too many other fruits by mistake. PR AUC is really good at showing this because it looks at precision (how many of the things the model says are red apples actually are red apples) and recall (how many of the red apples the model finds). When the red apples are rare, PR AUC gives you a better idea of how well your model is working.

In a situation with class imbalance, ROC AUC might not be as helpful. ROC AUC looks at how well the model can tell the difference between red apples and other fruits, but it doesn't focus as much on the rare red apples. This can make ROC AUC less useful when you really care about finding those few red apples. PR AUC, on the other hand, is better because it shows how well the model can balance finding the rare red apples (high recall) while not labeling too many other fruits as red apples (high precision). So, when you have a lot more of one thing than another in your data, PR AUC is a better choice to see how well your model is doing.

## What are the steps to calculate the PR AUC from a confusion matrix?

To calculate the PR AUC from a confusion matrix, you first need to understand that a confusion matrix shows how many times your model got things right and wrong. It has four parts: true positives (TP), which are the things your model correctly said were there; false positives (FP), which are the things your model said were there but weren't; true negatives (TN), which are the things your model correctly said weren't there; and false negatives (FN), which are the things your model missed. From the confusion matrix, you can calculate precision and recall at different thresholds. Precision is the number of true positives divided by the total number of positives your model predicted, which is $$ \text{Precision} = \frac{TP}{TP + FP} $$. Recall is the number of true positives divided by the total number of actual positives, which is $$ \text{Recall} = \frac{TP}{TP + FN} $$.

Once you have precision and recall at different thresholds, you can plot them on a graph to make the PR curve. The x-axis is recall, and the y-axis is precision. As you change the threshold, you get different values for precision and recall, and you plot these points to form the curve. The PR AUC is the area under this curve, which you can calculate using different methods like the trapezoidal rule. A higher PR AUC means your model is better at balancing finding the things it should find (high recall) and making sure the things it finds are actually correct (high precision).

## How can you use PR AUC to compare different models?

You can use PR AUC to compare different models by looking at how well each model balances finding the right things and making sure its guesses are correct. Imagine you have two models trying to find red apples in a pile of fruits. If Model A has a higher PR AUC than Model B, it means Model A is better at picking up most of the red apples (high recall) while also making sure that most of the fruits it picks up are actually red apples (high precision). This makes PR AUC a helpful number to compare models, especially when the thing you're looking for is rare.

To calculate PR AUC for comparison, you start by sorting the predictions by their confidence scores, from highest to lowest. For each prediction, you decide if it's a positive or negative example based on a threshold. As you move the threshold from high to low, you calculate the precision and recall at each point. Precision is the number of true positives divided by the total number of positives your model predicted, which is $$ \text{Precision} = \frac{TP}{TP + FP} $$. Recall is the number of true positives divided by the total number of actual positives, which is $$ \text{Recall} = \frac{TP}{TP + FN} $$. You plot these values on a graph, with recall on the x-axis and precision on the y-axis, to form the PR curve. The area under this curve, the PR AUC, gives you a single number that summarizes how well your model balances precision and recall across all thresholds. By comparing these PR AUC values, you can see which model does a better job at finding the rare things you care about.

## What are the limitations of using PR AUC as a performance metric?

PR AUC is a helpful way to see how well a model finds rare things while keeping its guesses correct, but it has some limits. One big limit is that PR AUC can be hard to understand for people who aren't used to it. It's not as simple as looking at one number like accuracy, where a higher number always means better. PR AUC needs a bit more work to understand because it's about balancing two things, precision and recall, and the shape of the curve matters a lot. If you don't know how to read the curve, you might miss important details about how well the model is doing.

Another limit is that PR AUC can be affected a lot by the data you use. If your data has a lot more of one type of thing than another, the PR AUC can look really good even if the model isn't that great. This is because PR AUC focuses on how well the model finds the rare things, but it might not show if the model is making a lot of mistakes with the common things. So, you need to be careful and use other ways to check the model's performance too, not just PR AUC.

## How can you optimize a model specifically for improving its PR AUC score?

To optimize a model for a better PR AUC score, you need to focus on balancing precision and recall. Precision is about how many of the things your model says are correct actually are correct. Recall is about how many of the correct things your model finds. You can do this by changing the threshold that decides what your model says is positive or negative. Try different thresholds and see how they change the precision and recall. You want to find a threshold that gives you a good balance between finding most of the right things (high recall) and making sure the things you find are actually right (high precision). You can use a technique called grid search to try out different thresholds and see which one gives the best PR AUC.

Another way to improve the PR AUC is by adjusting your model. You can change things like the model's complexity, the features you use, or even the type of model you're using. For example, if you're using a decision tree, you might try changing the tree's depth or the minimum number of samples needed at a leaf node. If you're using a [neural network](/wiki/neural-network), you might try adding more layers or changing the learning rate. You can use cross-validation to test these changes and see how they affect the PR AUC. By trying out different settings and seeing how they change the PR AUC, you can find the best way to set up your model to balance precision and recall.

## References & Further Reading

[1]: Saito, T., & Rehmsmeier, M. (2015). ["The Precision-Recall Plot is More Informative than the ROC Plot When Evaluating Binary Classifiers on Imbalanced Datasets."](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0118432) PLoS ONE, 10(3): e0118432.

[2]: Davis, J., & Goadrich, M. (2006). ["The Relationship Between Precision-Recall and ROC Curves."](https://dl.acm.org/doi/10.1145/1143844.1143874) In Proceedings of the 23rd International Conference on Machine Learning, pp. 233-240.

[3]: Fawcett, T. (2006). ["An Introduction to ROC Analysis."](https://www.sciencedirect.com/science/article/pii/S016786550500303X) Pattern Recognition Letters, 27(8), 861-874.

[4]: Boyd, K., Eng, K. H., & Page, C. D. (2013). ["Area Under the Precision-Recall Curve: Point Estimates and Confidence Intervals."](https://link.springer.com/chapter/10.1007/978-3-642-40994-3_29) In Proceedings of the 13th International Conference on Data Mining, pp. 451-459.

[5]: He, H., & Garcia, E. A. (2009). ["Learning from Imbalanced Data."](https://ieeexplore.ieee.org/document/5128907) IEEE Transactions on Knowledge and Data Engineering, 21(9), 1263-1284.

[6]: Manning, C. D., Raghavan, P., & Schütze, H. (2008). ["Introduction to Information Retrieval."](https://nlp.stanford.edu/IR-book/information-retrieval-book.html) Cambridge University Press.

[7]: Powers, D. M. W. (2011). ["Evaluation: From Precision, Recall and F-Measure to ROC, Informedness, Markedness & Correlation."](https://arxiv.org/abs/2010.16061) Journal of Machine Learning Technologies, 2(1), 37-63.