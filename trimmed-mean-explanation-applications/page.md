---
title: "Trimmed Mean: Explanation and Applications"
description: "Explore the concept of trimmed mean and its crucial applications in algorithmic trading Discover how trimming outliers improves trading strategy precision and outcomes"
---


![Image](images/1.png)

## Table of Contents

## What is a trimmed mean?

A trimmed mean is a way to find the average of a set of numbers by removing some of the highest and lowest values first. Imagine you have a list of test scores, and you want to find the average, but you think the very highest and lowest scores might not be typical. So, you decide to ignore, or "trim," a certain percentage of these extreme scores from both ends before calculating the average. This can give you a better idea of what a typical score might be.

For example, if you have 10 test scores and you decide to trim 10% from each end, you would remove the highest and lowest score. Then, you would calculate the average of the remaining 8 scores. This method helps to reduce the impact of outliers, which are numbers that are much higher or lower than the others, making the average more representative of the majority of the data.

## How is a trimmed mean calculated?

To calculate a trimmed mean, you first decide on a percentage of data points you want to trim from both the high and low ends of your data set. For example, if you choose to trim 10%, and you have 100 numbers, you would remove the highest 10 numbers and the lowest 10 numbers. This leaves you with the middle 80 numbers.

Next, you add up all the numbers that remain after trimming and then divide by the number of remaining numbers. So, if you trimmed 10% from each end of a set of 100 numbers, you would add up the middle 80 numbers and then divide by 80. This gives you the trimmed mean, which is a more representative average because it's not affected as much by very high or very low numbers.

## Why would someone use a trimmed mean instead of a regular mean?

Someone might use a trimmed mean instead of a regular mean because it can give a better picture of what's typical in a set of numbers. A regular mean, or average, can be pulled way up or way down by just a few numbers that are much higher or lower than the rest. These numbers are called outliers. If you have a few outliers, the regular mean might not show what's normal for most of the data. By trimming off the highest and lowest numbers, the trimmed mean focuses on the middle part of the data, which is often more useful.

For example, imagine you're looking at the salaries of people in a company. If the CEO makes a lot more money than everyone else, the regular mean salary might seem much higher than what most people actually earn. By using a trimmed mean, you can cut out the CEO's salary and maybe the lowest-paid worker's salary too. This way, the trimmed mean will be closer to what most employees earn, giving a clearer idea of typical salaries in the company.

## What are the advantages of using a trimmed mean?

Using a trimmed mean can help you get a better idea of what's normal in a set of numbers. When you use a regular mean, a few very high or very low numbers can make the average look different from what most of the numbers are like. By trimming off these extreme numbers, the trimmed mean focuses on the middle part of the data. This makes it a good choice when you want to see what's typical without being thrown off by outliers.

Another advantage is that a trimmed mean can be more reliable in certain situations. For example, if you're looking at test scores and a few students did much better or worse than everyone else, the regular mean might not show what most students scored. By using a trimmed mean, you can ignore those extreme scores and get a clearer picture of how the class did overall. This can be really helpful in making decisions based on the data, like figuring out if a class needs more help or if a test was too hard or too easy.

## What are the disadvantages of using a trimmed mean?

One problem with using a trimmed mean is that you have to decide how much to trim. If you trim too much, you might miss out on important information. If you don't trim enough, the extreme numbers can still affect your average. It's not always clear how much to trim, and different people might choose different amounts, which can lead to different results.

Another issue is that by trimming the data, you're throwing away some of it. This means you're not using all the information you have. Sometimes, those extreme numbers can be important, like if they show something unusual happening. By ignoring them, you might miss out on understanding the full story of your data.

## In what fields or scenarios is a trimmed mean commonly applied?

A trimmed mean is often used in fields like economics and finance. For example, when looking at income data, a few people might earn a lot more or a lot less than most others. Using a trimmed mean helps to see what most people earn without the very high or very low incomes changing the average too much. This can be useful for understanding things like average salaries in a company or a country.

In education, a trimmed mean can be helpful when looking at test scores. If a few students do much better or worse than the rest, the regular average might not show what most students scored. By trimming off the highest and lowest scores, teachers and schools can get a better idea of how the class did overall. This can help them decide if the class needs more help or if the test was too hard or too easy.

In sports, a trimmed mean can also be used to look at performance data. For instance, if you're looking at the times of runners in a race, a few might be much faster or slower than the others. By using a trimmed mean, you can see what the typical time was for most runners, which can help coaches understand the overall performance of the team.

## How does the choice of trimming percentage affect the trimmed mean?

The choice of trimming percentage can really change the trimmed mean. If you trim a lot, you're cutting off more of the highest and lowest numbers. This makes the trimmed mean focus more on the middle numbers, which can be good if you want to see what's typical without being affected by extreme numbers. But if you trim too much, you might miss out on important information that those extreme numbers could tell you.

On the other hand, if you trim just a little, the trimmed mean will be closer to the regular mean. This means the extreme numbers can still have some effect on your average. It's a balance - you want to trim enough to get rid of the outliers that might mess up your average, but not so much that you lose the full picture of your data. The right amount of trimming depends on what you're trying to find out from your data.

## Can you provide an example of calculating a trimmed mean with a real dataset?

Let's say we have a small dataset of test scores from a class: 50, 60, 65, 70, 75, 80, 85, 90, 95, 100. We want to calculate a 10% trimmed mean. Since we have 10 scores, trimming 10% from each end means we'll remove the highest score (100) and the lowest score (50). This leaves us with the scores: 60, 65, 70, 75, 80, 85, 90, 95.

Now, we add up these remaining scores: 60 + 65 + 70 + 75 + 80 + 85 + 90 + 95 = 620. Since we trimmed off 2 scores, we have 8 scores left. To find the trimmed mean, we divide the total by the number of remaining scores: 620 ÷ 8 = 77.5. So, the 10% trimmed mean of these test scores is 77.5. This gives us a better idea of what most students scored, without the highest and lowest scores affecting the average too much.

## How does a trimmed mean compare to other measures of central tendency like median and mode?

A trimmed mean is different from the median and the mode because it's a way to find the average that cuts out some of the highest and lowest numbers first. The median is the middle number when you line up all the numbers from smallest to biggest. It doesn't care about the other numbers, just the one in the middle. The mode is the number that shows up the most in your list. It can be useful when you want to know what's most common, but it might not tell you much if there are a lot of different numbers. A trimmed mean, on the other hand, gives you an average that's not pulled around by a few very high or very low numbers, which can be helpful when you want to see what's typical for most of your data.

The choice between using a trimmed mean, median, or mode depends on what you're trying to find out. If you want to know what most people scored on a test, and you think a few really high or low scores might mess up your average, a trimmed mean could be a good choice. It's like a regular average but without the extremes. The median is good when you want to know the middle value and don't want any numbers to affect your answer too much. The mode is useful when you want to know what happens most often, but it might not be helpful if your data has a lot of different numbers or if no number shows up more than once. Each measure has its own way of showing what's typical in a set of numbers, and the best one to use depends on your data and what you're trying to learn from it.

## What are the statistical properties of a trimmed mean?

A trimmed mean has some special properties that make it different from a regular mean. One important property is that it's less affected by outliers, which are numbers that are much higher or lower than the rest. When you trim off a certain percentage of the highest and lowest numbers, the trimmed mean focuses more on the middle part of your data. This can make it a better way to see what's typical for most of your numbers, especially if you have a few extreme values that could pull the regular mean in one direction or another.

Another property of a trimmed mean is that it can be more stable than a regular mean. This means that if you add or remove a few numbers from your dataset, the trimmed mean might not change as much as the regular mean would. This stability can be really helpful when you're working with data that might have some errors or unusual values. However, the exact amount of stability depends on how much you trim. If you trim too much, you might lose important information, and if you don't trim enough, the extreme numbers can still affect your average. So, choosing the right amount to trim is important for getting the most out of a trimmed mean.

## How can trimmed means be used in robust statistical analysis?

In robust statistical analysis, a trimmed mean is used to get a better idea of what's typical in a set of numbers, even when there are some unusual or extreme values. These extreme values, called outliers, can make the regular mean, or average, look different from what most of the numbers are like. By trimming off a certain percentage of the highest and lowest numbers, a trimmed mean focuses on the middle part of the data. This makes it a good choice when you want to see what's normal without being thrown off by outliers.

For example, if you're looking at the salaries of people in a company, and the CEO makes a lot more money than everyone else, the regular mean salary might seem much higher than what most people actually earn. By using a trimmed mean, you can cut out the CEO's salary and maybe the lowest-paid worker's salary too. This way, the trimmed mean will be closer to what most employees earn, giving a clearer idea of typical salaries in the company. This makes the trimmed mean a useful tool in robust statistical analysis, where the goal is to understand the data without being misled by a few extreme values.

## What advanced techniques or variations exist for calculating trimmed means in specialized applications?

In specialized applications, there are advanced techniques for calculating trimmed means that can make them even more useful. One variation is the winsorized mean, where instead of cutting out the highest and lowest numbers, you replace them with the next highest or lowest number that's still in the data. This can be helpful when you want to keep all your data but still reduce the effect of outliers. Another technique is the adaptive trimmed mean, where the amount of trimming changes based on how spread out the numbers are. If the numbers are very spread out, you might trim more to focus on the middle part of the data.

These advanced techniques can be really helpful in fields like finance or medicine, where the data can have a lot of extreme values. For example, in finance, stock prices can jump around a lot, and in medicine, test results can vary widely from person to person. By using these special kinds of trimmed means, you can get a better idea of what's typical without being thrown off by a few unusual numbers. This can help you make better decisions based on the data, like figuring out if a stock is a good investment or if a medical treatment is working well for most people.

## References & Further Reading

[1]: ["Advances in Financial Machine Learning"](https://www.amazon.com/Advances-Financial-Machine-Learning-Marcos/dp/1119482089) by Marcos Lopez de Prado

[2]: ["Evidence-Based Technical Analysis: Applying the Scientific Method and Statistical Inference to Trading Signals"](https://www.amazon.com/Evidence-Based-Technical-Analysis-Scientific-Statistical/dp/0470008741) by David Aronson

[3]: ["Machine Learning for Algorithmic Trading"](https://github.com/stefan-jansen/machine-learning-for-trading) by Stefan Jansen

[4]: ["Quantitative Trading: How to Build Your Own Algorithmic Trading Business"](https://www.amazon.com/Quantitative-Trading-Build-Algorithmic-Business/dp/1119800064) by Ernest P. Chan

[5]: Hampel, F. R. (1974). ["The Influence Curve and Its Role in Robust Estimation."](https://www.jstor.org/stable/2285666) The Annals of Statistics, 2(3), 377-395.

[6]: Tukey, J. W. (1977). ["Exploratory Data Analysis."](https://archive.org/details/exploratorydataa0000tuke_7616) Addison-Wesley.