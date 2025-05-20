---
category: quant_concept
description: F1 Score measures balanced precision and recall for imbalanced classification
  tasks including medical diagnosis and fraud detection Discover more inside
title: Comprehensive Guide to F1 Score in Machine Learning
---

![Image](images/1.webp)

## Table of Contents

## What is F1 score in machine learning?

The F1 score is a way to measure how well a machine learning model is doing, especially when the data is not balanced. It combines two other important measures: precision and recall. Precision is about how many of the items the model said were correct actually were correct. Recall is about how many of the correct items the model was able to find. The F1 score is the harmonic mean of precision and recall, which means it gives a single number that considers both of these measures equally. The formula for the F1 score is $$F1 = 2 \times \frac{\text{precision} \times \text{recall}}{\text{precision} + \text{recall}}$$. The F1 score ranges from 0 to 1, where a score of 1 means the model is perfect, and a score of 0 means the model is doing very badly.

The F1 score is really useful when you want to balance the importance of precision and recall. For example, in medical diagnosis, you want to catch all the sick people (high recall) but also make sure that the people you say are sick really are sick (high precision). The F1 score helps you see how well your model is doing at both of these things at the same time. If your model has a high F1 score, it means it's doing a good job at finding the right balance between precision and recall. If the F1 score is low, it means your model might be good at one but not the other, and you might need to adjust your model to improve its performance.

## How is the F1 score calculated?

The F1 score is calculated by using two other measures: precision and recall. Precision tells us how many of the items the model said were correct actually were correct. It's like saying if the model says something is a cat, how often is it really a cat? Recall tells us how many of the correct items the model was able to find. It's like saying if there are 10 cats, how many of those 10 did the model find? To get the F1 score, we use both precision and recall together.

The formula for the F1 score is $$F1 = 2 \times \frac{\text{precision} \times \text{recall}}{\text{precision} + \text{recall}}$$. This formula takes the harmonic mean of precision and recall, which means it gives a score that considers both measures equally. The F1 score ranges from 0 to 1. A score of 1 means the model is perfect at balancing precision and recall, and a score of 0 means the model is doing very badly. So, if you want to see how well your model is doing at finding the right things and not making mistakes, the F1 score is a good way to check.

## Why is the F1 score important in classification problems?

The F1 score is important in classification problems because it helps us see how well a model is doing when the data is not balanced. Imagine you have a lot of pictures, and most of them are dogs, but only a few are cats. A model might say all pictures are dogs just to be safe, and it would be right most of the time. But that's not helpful if you really need to find the cats. The F1 score looks at both how many cats the model finds (recall) and how many of the pictures it says are cats really are cats (precision). This way, the F1 score gives us a better idea of the model's true performance.

The formula for the F1 score is $$F1 = 2 \times \frac{\text{precision} \times \text{recall}}{\text{precision} + \text{recall}}$$. This formula balances precision and recall equally, which is really useful when you want to make sure your model is good at both finding the right things and not making too many mistakes. If the F1 score is high, it means your model is doing a good job at this balance. If it's low, it might mean your model is good at one thing but not the other, and you might need to adjust your model to improve its performance. So, the F1 score is a helpful tool to check how well your model is working, especially in situations where finding all the right things is as important as not making mistakes.

## What are the differences between precision, recall, and F1 score?

Precision, recall, and F1 score are all ways to measure how well a [machine learning](/wiki/machine-learning) model is doing, but they look at different things. Precision is about how many of the items the model said were correct actually were correct. For example, if the model says 10 pictures are cats, and 8 of them really are cats, the precision is 80%. Recall is about how many of the correct items the model was able to find. If there are 20 cats in total and the model finds 16 of them, the recall is 80%. Precision and recall focus on different aspects of the model's performance, with precision focusing on the accuracy of the positive predictions and recall focusing on the completeness of finding all positive instances.

The F1 score combines precision and recall into one number. It's the harmonic mean of precision and recall, which means it gives a score that considers both measures equally. The formula for the F1 score is $$F1 = 2 \times \frac{\text{precision} \times \text{recall}}{\text{precision} + \text{recall}}$$. The F1 score is useful when you want to balance the importance of precision and recall. For example, in medical diagnosis, you want to catch all the sick people (high recall) but also make sure that the people you say are sick really are sick (high precision). The F1 score helps you see how well your model is doing at both of these things at the same time. If your model has a high F1 score, it means it's doing a good job at finding the right balance between precision and recall.

## In what scenarios is F1 score particularly useful?

The F1 score is really useful when you're dealing with data that isn't balanced. Imagine you're trying to find rare items, like spotting a few cats in a sea of dogs. A model might just say everything is a dog to be safe, and it would be right most of the time. But that's not helpful if you really need to find those cats. The F1 score helps by looking at how many cats the model finds (recall) and how many of the things it says are cats really are cats (precision). It's like getting the best of both worlds, making sure the model is good at finding the right things and not making too many mistakes.

The F1 score is also great when you want to make sure your model is doing well at both finding all the right things and being accurate. For example, in medical tests, you want to catch all the sick people (high recall) but also make sure the people you say are sick really are sick (high precision). The F1 score combines these two things into one number using the formula $$F1 = 2 \times \frac{\text{precision} \times \text{recall}}{\text{precision} + \text{recall}}$$. If the F1 score is high, it means your model is doing a good job at this balance. If it's low, it might mean your model is good at one thing but not the other, and you might need to adjust your model to improve its performance.

## How does F1 score handle imbalanced datasets?

The F1 score is really good at dealing with imbalanced datasets. Imagine you have a lot of pictures, and most of them are dogs, but only a few are cats. A model might say all pictures are dogs just to be safe, and it would be right most of the time. But that's not helpful if you really need to find the cats. The F1 score looks at both how many cats the model finds (recall) and how many of the pictures it says are cats really are cats (precision). This way, it gives us a better idea of how well the model is doing, even when there are way more dogs than cats.

The F1 score is calculated using the formula $$F1 = 2 \times \frac{\text{precision} \times \text{recall}}{\text{precision} + \text{recall}}$$. This formula balances precision and recall equally, which is really useful when you want to make sure your model is good at both finding the right things and not making too many mistakes. If the F1 score is high, it means your model is doing a good job at this balance. If it's low, it might mean your model is good at one thing but not the other, and you might need to adjust your model to improve its performance. So, the F1 score is a helpful tool to check how well your model is working, especially in situations where finding all the right things is as important as not making mistakes.

## Can you explain the harmonic mean used in F1 score?

The harmonic mean is a way of finding an average that's used in the F1 score. It's different from the regular average, which you might know as the arithmetic mean. The harmonic mean is used when you want to give more weight to smaller numbers. For the F1 score, it's used to balance precision and recall. The formula for the harmonic mean of two numbers, like precision and recall, is $$ \text{Harmonic Mean} = \frac{2 \times \text{precision} \times \text{recall}}{\text{precision} + \text{recall}} $$. This means the F1 score will be lower if either precision or recall is low, even if the other one is high.

Using the harmonic mean in the F1 score makes sure that both precision and recall are important. If you only used the regular average, a model could have a high score just by being good at one thing and bad at the other. But with the harmonic mean, the F1 score will be low if the model is bad at either finding all the right things (recall) or being accurate (precision). This makes the F1 score a fair way to see how well a model is doing, especially when the data is not balanced.

## What are the limitations of using F1 score as a metric?

The F1 score is really helpful, but it has some limitations. One big problem is that it only works well when you're looking at just two categories, like cats and dogs. If you have more than two categories, like cats, dogs, and birds, the F1 score can't handle it as easily. You'd need to calculate an F1 score for each category and then figure out how to combine them, which can be tricky.

Another limitation is that the F1 score treats precision and recall as equally important. But sometimes, one might be more important than the other. For example, in medical tests, it might be more important to find all the sick people (high recall) than to be super accurate about who's sick (high precision). The F1 score, with its formula $$F1 = 2 \times \frac{\text{precision} \times \text{recall}}{\text{precision} + \text{recall}}$$, doesn't let you change how much you care about precision versus recall. So, if you need to focus more on one over the other, the F1 score might not be the best choice.

Lastly, the F1 score can be hard to understand for people who aren't used to it. It's a single number that combines two other measures, and it can be confusing to know what a certain F1 score really means. If you're trying to explain how well a model is doing to someone who doesn't know much about machine learning, the F1 score might not be the easiest way to do that.

## How can F1 score be used in multi-class classification?

In multi-class classification, where you have more than two categories, the F1 score can still be used but it needs to be calculated differently. Instead of just one F1 score, you calculate an F1 score for each category. For example, if you're classifying pictures into cats, dogs, and birds, you would calculate an F1 score for cats, an F1 score for dogs, and an F1 score for birds. Each of these F1 scores tells you how well the model is doing for that specific category, looking at both how many of that category the model finds (recall) and how many of the things it says are in that category really are (precision). The formula for the F1 score is still $$F1 = 2 \times \frac{\text{precision} \times \text{recall}}{\text{precision} + \text{recall}}$$, but you use it separately for each category.

Once you have the F1 scores for each category, you need to combine them into one overall score if you want to see how the model is doing across all categories. There are a few ways to do this. One common way is to take the average of all the F1 scores. This is called the macro-average F1 score. Another way is to calculate the F1 score for each category, but then weigh them based on how many examples of each category there are in the data. This is called the weighted-average F1 score. Both of these methods give you a single number that tells you how well the model is doing overall, but they look at the data in slightly different ways.

## What are some alternatives to F1 score and when might they be preferred?

One alternative to the F1 score is the Area Under the Receiver Operating Characteristic Curve (AUC-ROC). The AUC-ROC looks at how well a model can tell the difference between two categories, like cats and dogs. It's a good choice when you want to see how well your model is doing at different levels of confidence. The AUC-ROC is a number between 0 and 1, where 1 means the model is perfect at telling the difference between the categories. It's especially useful when your data is not balanced, because it doesn't care about the actual number of cats and dogs, just how well the model can tell them apart.

Another alternative is the Matthews Correlation Coefficient (MCC). The MCC is like a score that tells you how well your model is doing, but it's different from the F1 score because it looks at all four parts of the confusion matrix: true positives, true negatives, false positives, and false negatives. The formula for MCC is $$ \text{MCC} = \frac{TP \times TN - FP \times FN}{\sqrt{(TP + FP)(TP + FN)(TN + FP)(TN + FN)}} $$, where TP is true positives, TN is true negatives, FP is false positives, and FN is false negatives. The MCC is good when you want to see how well your model is doing overall, and it's especially useful when your data is not balanced. It gives you a number between -1 and 1, where 1 means the model is perfect, 0 means it's doing no better than guessing, and -1 means it's doing the opposite of what it should.

A third alternative is the Cohen's Kappa score. Cohen's Kappa looks at how well your model agrees with the real answers, but it also takes into account how much agreement you would expect by chance. It's a good choice when you want to see how much better your model is doing than just guessing. The formula for Cohen's Kappa is $$ \kappa = \frac{p_o - p_e}{1 - p_e} $$, where $p_o$ is the observed agreement and $p_e$ is the expected agreement by chance. Cohen's Kappa is useful when you want to see how well your model is doing, especially when the data is not balanced, and it's good for comparing different models or different people's predictions.

## How does F1 score relate to the ROC curve and AUC?

The F1 score and the ROC curve (Receiver Operating Characteristic curve) along with its AUC (Area Under the Curve) are both ways to measure how well a machine learning model is doing, but they look at different things. The F1 score is a single number that combines precision and recall. Precision is about how many of the things the model says are correct really are correct, and recall is about how many of the correct things the model finds. The formula for the F1 score is $$F1 = 2 \times \frac{\text{precision} \times \text{recall}}{\text{precision} + \text{recall}}$$. The F1 score is really useful when you want to see how well the model is doing at finding the right things and not making too many mistakes, especially when the data is not balanced.

The ROC curve and AUC, on the other hand, look at how well the model can tell the difference between two categories at different levels of confidence. The ROC curve is a graph that shows how the model's performance changes as you change how sure the model needs to be to say something is in one category. The AUC is a number between 0 and 1 that tells you how good the model is overall. A higher AUC means the model is better at telling the categories apart. The ROC curve and AUC are good when you want to see how well the model is doing at different levels of confidence, and they're especially useful when the data is not balanced. While the F1 score gives you one number that balances precision and recall, the ROC curve and AUC give you a more detailed look at how the model performs at different levels of confidence.

## What advanced techniques can be used to optimize F1 score in model tuning?

To optimize the F1 score in model tuning, one effective technique is to use cross-validation. This method splits your data into different parts and trains the model on some of the parts while testing it on others. By doing this many times with different splits, you can get a good idea of how well your model is doing on average. You can then adjust your model's settings, like the learning rate or the number of layers in a [neural network](/wiki/neural-network), to see if the F1 score goes up. Another technique is to use grid search or random search to try out different combinations of settings. For example, you might try different values for the learning rate and see which one gives the best F1 score. This can help you find the best settings for your model without having to guess.

Another advanced technique is to use class weighting. If your data is not balanced, meaning you have a lot more examples of one category than another, you can tell your model to pay more attention to the less common category. This can help improve the F1 score by making sure the model is good at finding all the right things (recall) and being accurate (precision). You can do this by setting weights in your model's settings. For example, if you have a lot more dogs than cats, you might set a higher weight for cats to make sure the model doesn't ignore them. The formula for the F1 score is $$F1 = 2 \times \frac{\text{precision} \times \text{recall}}{\text{precision} + \text{recall}}$$, and by using class weighting, you can help balance the precision and recall to get a higher F1 score.

## References & Further Reading

[1]: Sokolova, M., & Lapalme, G. (2009). ["A systematic analysis of performance measures for classification tasks."](https://www.sciencedirect.com/science/article/pii/S0306457309000259) Information Processing & Management, 45(4), 427-437.

[2]: Powers, D. M. W. (2011). ["Evaluation: From Precision, Recall and F-Measure to ROC, Informedness, Markedness & Correlation."](https://arxiv.org/abs/2010.16061) Journal of Machine Learning Technologies, 2(1), 37-63.

[3]: Flach, P. (2019). ["Performance Evaluation in Machine Learning: The Good, the Bad, the Ugly."](https://ojs.aaai.org/index.php/AAAI/article/view/5055) Proceedings of the 42nd International ACM SIGIR Conference on Research and Development in Information Retrieval.

[4]: Hanley, J. A., & McNeil, B. J. (1982). ["The meaning and use of the area under a receiver operating characteristic (ROC) curve."](https://pubmed.ncbi.nlm.nih.gov/7063747/) Radiology, 143(1), 29-36.

[5]: Chicco, D., & Jurman, G. (2020). ["The advantages of the Matthews Correlation Coefficient (MCC) over F1 score and accuracy in binary classification evaluation."](https://pubmed.ncbi.nlm.nih.gov/31898477/) PeerJ.