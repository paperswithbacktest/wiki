---
category: dataset
description: Undersampling in machine learning balances datasets by trimming majority
  class data to improve model fairness and generalization Discover more inside
title: Effective Undersampling Techniques for Machine Learning Models
---

![Image](images/1.jpeg)

## Table of Contents

## What is undersampling in machine learning?

Undersampling is a technique used in machine learning to balance datasets where one class has a lot more examples than the other. When you have a dataset with imbalanced classes, it can be hard for a model to learn well because it sees much more of one class than the other. So, undersampling helps by reducing the number of examples from the larger class to match the smaller one. For example, if you have 1000 examples of class A and 100 of class B, you might randomly remove some examples from class A until you have 100 of each.

This method can make the model perform better on both classes because it gets to see an equal number of examples from each. However, a downside of undersampling is that you throw away data, which might mean losing useful information. Also, if you don't choose the examples to remove carefully, you might end up with a less diverse set of examples, which can affect how well your model generalizes to new data. So, while undersampling can be helpful, it's important to use it thoughtfully and consider other methods like oversampling or using special algorithms designed for imbalanced data.

## Why is undersampling used in machine learning?

Undersampling is used in machine learning to fix a problem where one type of data (class) is much more common than another. Imagine you're trying to teach a computer to tell the difference between cats and dogs, but you have way more pictures of dogs. The computer might get really good at recognizing dogs but not so good with cats. By using undersampling, you take away some of the dog pictures so that you have an equal number of cat and dog pictures. This helps the computer learn about both cats and dogs equally well.

However, undersampling has its downsides. When you remove data, you might lose important information that could help the computer learn better. Also, if you're not careful about which data you remove, you might end up with a less varied set of examples. This can make it harder for the computer to understand new pictures it hasn't seen before. So, while undersampling can help balance the data, it's important to think carefully about how you do it and consider other methods like adding more data or using special techniques designed for this kind of problem.

## What are the common scenarios where undersampling is applied?

Undersampling is often used when you have a lot more examples of one thing than another in your data. For example, in a bank's fraud detection system, there might be thousands of normal transactions for every single fraudulent one. If you train a computer model on this data without balancing it, the model might get really good at spotting normal transactions but miss the fraud because it didn't see enough examples of it. By using undersampling, you can reduce the number of normal transactions to match the number of fraud cases, helping the model learn about both types equally well.

Another common scenario is in medical diagnosis, where diseases might be rare compared to healthy cases. If you're trying to teach a computer to spot a rare disease from medical images, having way more images of healthy patients can make the model focus too much on what's common and not learn well about the disease. Undersampling can help by cutting down the number of healthy images to match the number of disease images, giving the model a fair chance to learn about both.

In both cases, the goal is to make the data more balanced so the computer can learn better. However, it's important to be careful with undersampling because you're throwing away data, which might mean losing important information. Sometimes, other methods like oversampling or using special algorithms designed for imbalanced data might be better choices.

## How does undersampling affect the performance of a machine learning model?

Undersampling can help a [machine learning](/wiki/machine-learning) model perform better when dealing with imbalanced data. By reducing the number of examples from the larger class to match the smaller one, the model gets a chance to learn about both classes equally well. For example, if you're trying to spot rare events like fraud, undersampling the common non-fraud cases can make the model pay more attention to the fraud cases, improving its ability to catch them.

However, undersampling also has its downsides. When you throw away data, you might lose important information that could help the model learn better. Also, if you're not careful about which data you remove, you might end up with a less varied set of examples. This can make the model less good at understanding new data it hasn't seen before, which can hurt its overall performance. So, while undersampling can be helpful, it's important to use it carefully and consider other methods like oversampling or special algorithms designed for imbalanced data.

## What are the different techniques used for undersampling?

Undersampling is a way to balance data where one type is much more common than another. One common technique is random undersampling, where you simply remove examples from the larger class at random until you have the same number as the smaller class. This is easy to do but can lead to losing important information because you're not choosing which examples to keep based on anything other than luck.

Another technique is called Tomek Links, which focuses on removing examples that are close to the boundary between the two classes. By removing these, you help make the separation between classes clearer, which can help the model learn better. This method can be more thoughtful than random undersampling because it looks at how examples relate to each other.

There's also a method called Cluster Centroids, which works by grouping similar examples together into clusters and then keeping only the center of each cluster. This way, you keep a diverse set of examples while still reducing the total number. Each of these methods has its own way of trying to balance the data while keeping as much useful information as possible.

## Can you explain the Random Undersampling method?

Random undersampling is a way to balance data where one type of thing is much more common than another. Imagine you have a lot more pictures of dogs than cats. To help the computer learn about both equally well, you can use random undersampling to take away some dog pictures until you have the same number of dog and cat pictures. You do this by choosing which dog pictures to remove completely by chance, like [picking](/wiki/asset-class-picking) numbers out of a hat.

This method is easy to do because you don't need to think too hard about which pictures to keep or throw away. You just let luck decide. But there's a downside: by removing pictures randomly, you might accidentally get rid of important ones that could help the computer learn better. So, while random undersampling can help balance the data, it's important to be careful and maybe try other methods too, like adding more cat pictures or using special computer tricks designed for this kind of problem.

## What are the advantages and disadvantages of using undersampling?

Undersampling helps balance data when one type of thing is much more common than another. For example, if you have a lot more pictures of dogs than cats, undersampling can help by taking away some dog pictures so you have the same number of each. This makes it easier for the computer to learn about both dogs and cats equally well. By doing this, the computer can get better at recognizing the less common thing, like spotting rare events such as fraud in a bank's system.

However, undersampling has its downsides. When you remove data, you might lose important information that could help the computer learn better. If you're not careful about which data you remove, you might end up with a less varied set of examples. This can make the computer struggle to understand new data it hasn't seen before, which can hurt how well it performs overall. So, while undersampling can be helpful, it's important to use it carefully and consider other methods like adding more data or using special computer tricks designed for imbalanced data.

## How does undersampling compare to oversampling?

Undersampling and oversampling are two ways to fix the problem where one type of thing in your data is much more common than another. Undersampling works by taking away some of the common things until you have the same number of each type. For example, if you have a lot more pictures of dogs than cats, you might remove some dog pictures so you have an equal number of dog and cat pictures. This helps the computer learn about both dogs and cats equally well. But, by removing data, you might lose important information that could help the computer learn better. If you're not careful about which data you remove, the computer might struggle to understand new data it hasn't seen before.

Oversampling, on the other hand, works by adding more of the less common things until you have the same number as the more common ones. Using the same example, if you have fewer pictures of cats than dogs, you might make more cat pictures by copying the ones you already have or creating new ones that look similar. This way, the computer gets to see more cat pictures and can learn about them better. However, oversampling can lead to the computer overfitting, which means it might get too good at recognizing the copied or similar pictures but not as good with new, different ones. So, while both undersampling and oversampling can help balance data, they each have their own pros and cons, and it's important to choose the right method based on your specific situation.

## What is Tomek Links undersampling and how is it implemented?

Tomek Links undersampling is a way to balance data when one type of thing is much more common than another. Imagine you have a lot more pictures of dogs than cats. Tomek Links help by removing some dog pictures that are close to the cat pictures. These close dog pictures are called Tomek Links. By removing them, you make the space between dogs and cats clearer, which can help the computer learn better about both.

To implement Tomek Links undersampling, you first need to find the pairs of examples from different classes that are closest to each other. If you have a dog picture and a cat picture that are really close, that's a Tomek Link. You then remove the dog picture from the pair. Here's a simple example of how you might do this in Python:

```python
from sklearn.neighbors import NearestNeighbors
import numpy as np

def tomek_links_undersampling(X, y):
    nn = NearestNeighbors(n_neighbors=1)
    nn.fit(X[y == 0])  # Assuming 0 is the majority class
    distances, indices = nn.kneighbors(X[y == 1])  # Assuming 1 is the minority class

    tomek_links = []
    for i, (dist, idx) in enumerate(zip(distances.flatten(), indices.flatten())):
        if y[i] == 1 and y[idx] == 0:
            tomek_links.append((i, idx))

    # Remove the majority class instances that form Tomek Links
    tomek_indices = [idx for _, idx in tomek_links]
    mask = np.ones(len(X), dtype=bool)
    mask[tomek_indices] = False

    return X[mask], y[mask]

# Example usage
X = np.array([[1, 2], [2, 2], [3, 3], [4, 4], [5, 5]])
y = np.array([0, 0, 0, 1, 1])  # 0 is majority, 1 is minority
X_resampled, y_resampled = tomek_links_undersampling(X, y)
print("Resampled X:", X_resampled)
print("Resampled y:", y_resampled)
```

This code finds the Tomek Links and removes the majority class instances that form these links, helping to balance the dataset.

## How can you evaluate the effectiveness of undersampling in a dataset?

To evaluate how well undersampling works on a dataset, you need to see if it helps the computer model learn better about both common and rare things. One way to do this is by looking at how well the model can tell the difference between the two types of things after you've balanced the data. You can use measures like accuracy, which shows how often the model gets it right, or the F1 score, which is a balance between how well it spots the rare things and how often it's right when it says something is rare. If these measures go up after undersampling, it's a sign that the method helped.

Another way to check is by using something called a confusion matrix. This is like a table that shows how many times the model got each type of thing right or wrong. If the model is better at spotting the rare things after you use undersampling, you'll see more correct guesses in the confusion matrix for the rare class. You can also split your data into two parts: one part to train the model and another part to test it. If the model does better on the test part after undersampling, it's a good sign that the method worked well.

## What are some advanced undersampling techniques used in imbalanced datasets?

Undersampling is a way to balance data when one type of thing is much more common than another. One advanced technique is called Cluster Centroids. Imagine you have a lot more pictures of dogs than cats. Instead of just removing dog pictures at random, Cluster Centroids groups similar dog pictures together into clusters and then keeps only the picture that's in the middle of each cluster. This way, you keep a diverse set of dog pictures while still reducing the total number. This can help the computer learn better because it sees a good variety of dog pictures, even though there are fewer of them.

Another advanced method is called Edited Nearest Neighbors (ENN). ENN looks at each picture and checks its closest neighbors. If a dog picture is surrounded by more cat pictures than dog pictures, it might be confusing the computer, so ENN removes that dog picture. This helps make the space between dogs and cats clearer, which can help the computer learn better. Both of these methods try to keep important information while balancing the data, which can make the computer model perform better on both types of things.

## How can undersampling be integrated into a machine learning pipeline?

Undersampling can be added to a machine learning pipeline to help balance data where one type of thing is much more common than another. Imagine you're teaching a computer to tell the difference between dogs and cats, but you have a lot more pictures of dogs. You can use undersampling to take away some dog pictures until you have the same number of dog and cat pictures. This helps the computer learn about both dogs and cats equally well. To do this in your pipeline, you would first split your data into training and testing sets. Then, before you train your model, you apply the undersampling technique to the training set to make it balanced. After that, you train your model on this balanced data and then test it on the original, imbalanced test set to see how well it performs.

One way to add undersampling into your pipeline is by using Python with libraries like `imbalanced-learn`. For example, you might use random undersampling, which removes dog pictures at random until you have an equal number of dog and cat pictures. Here's a simple example of how you might do this:

```python
from sklearn.model_selection import train_test_split
from imblearn.under_sampling import RandomUnderSampler
from sklearn.datasets import make_classification
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import accuracy_score

# Create an imbalanced dataset
X, y = make_classification(n_samples=1000, n_classes=2, weights=[0.9, 0.1], random_state=42)

# Split the data into training and testing sets
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

# Apply random undersampling to the training data
rus = RandomUnderSampler(random_state=42)
X_resampled, y_resampled = rus.fit_resample(X_train, y_train)

# Train a model on the resampled data
model = RandomForestClassifier(random_state=42)
model.fit(X_resampled, y_resampled)

# Test the model on the original test set
y_pred = model.predict(X_test)
accuracy = accuracy_score(y_test, y_pred)
print(f"Accuracy on test set: {accuracy}")
```

This code shows how you can split your data, apply random undersampling to the training set, train a model on the balanced data, and then test it on the original test set to see how well it performs. By doing this, you help the computer learn better about both types of things in your data.

## References & Further Reading

[1]: He, H., & Garcia, E. A. (2009). ["Learning from Imbalanced Data."](https://ieeexplore.ieee.org/document/5128907) IEEE Transactions on Knowledge and Data Engineering.

[2]: Japkowicz, N., & Stephen, S. (2002). ["The class imbalance problem: A systematic study."](https://dl.acm.org/doi/10.5555/1293951.1293954) Intelligent Data Analysis.

[3]: Chawla, N. V., Bowyer, K. W., Hall, L. O., & Kegelmeyer, W. P. (2002). ["SMOTE: Synthetic Minority Over-sampling Technique."](https://arxiv.org/abs/1106.1813) Journal of Artificial Intelligence Research. 

[4]: Fernández, A., Garcia, S., Galar, M., Prati, R. C., Krawczyk, B., & Herrera, F. (2018). ["Learning from Imbalanced Data Sets."](https://link.springer.com/book/10.1007/978-3-319-98074-4) Springer International Publishing.

[5]: Van Hulse, J., Khoshgoftaar, T. M., & Napolitano, A. (2007). ["Experimental perspectives on learning from imbalanced data."](https://www.researchgate.net/publication/221344823_Experimental_Perspectives_on_Learning_from_Imbalanced_Data) Proceedings of the 24th International Conference on Machine Learning.