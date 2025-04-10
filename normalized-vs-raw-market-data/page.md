---
title: "Normalized vs Raw Market Data"
description: Explore the critical role of market data in algorithmic trading and the choice between normalized versus raw data. Normalized market data offers a standardized, streamlined approach for easier integration with trading strategies, while raw data provides comprehensive, unprocessed details directly from market feeds. This article investigates into the advantages and challenges of each data type, helping traders decide which aligns best with their goals and technical capabilities. Understanding these differences is key to developing effective and efficient trading strategies and enhancing overall performance in the fast-paced world of algo trading.
---


![Image](images/1.webp)

## Table of Contents

## What is market data?

Market data is information about what's happening in the world of buying and selling. This includes prices of stocks, bonds, commodities, and other financial products. People use market data to make smart choices about investing their money. It tells them how much things cost right now and how those costs have changed over time.

This data comes from many places, like stock exchanges, financial news services, and trading platforms. It's usually shown in real-time, which means it updates very quickly as new trades happen. Market data can be simple, like the current price of a stock, or more complex, like charts and graphs that show trends over time. By looking at this data, investors can decide when to buy or sell, trying to make a profit or avoid losses.

## What is the difference between normalized and raw market data?

Raw market data is the original information that comes straight from the market. It includes things like the prices of stocks, the number of shares traded, and the times of those trades. This data is not changed or fixed up in any way. It's like looking at a messy room where everything is just as it was left, with no tidying up.

Normalized market data, on the other hand, is raw data that has been cleaned up and made easier to understand. People take the raw data and adjust it so that it fits a common standard. This makes it simpler to compare different pieces of data. It's like cleaning up that messy room, organizing everything, and putting things in neat piles so you can see what you have more clearly. Normalized data helps people make better decisions because it's easier to see patterns and trends.

## Why is normalization of market data important?

Normalization of market data is important because it makes different pieces of data easier to compare. Imagine you have prices from different stock markets around the world. These prices might be in different currencies or use different scales. By normalizing the data, you can put everything on the same scale, making it easier to see which stocks are doing better or worse, no matter where they are from.

Also, normalization helps in spotting trends and patterns more clearly. Raw data can be messy and hard to understand because it includes a lot of noise and variations. When you normalize the data, you clean it up and make it smoother. This way, investors and analysts can see the big picture more easily and make smarter decisions about buying and selling.

## How is raw market data typically collected?

Raw market data is collected from many places where buying and selling happens. The main sources are stock exchanges, like the New York Stock Exchange or NASDAQ. These places keep track of every trade that happens, including the price, the number of shares, and the time of the trade. Financial news services and trading platforms also collect this data. They use special computer systems to gather information as soon as trades happen, making sure the data is as up-to-date as possible.

Once the data is collected, it is sent to data providers and financial institutions. These organizations use the data to help people make decisions about investing. The data is often sent through special networks that can handle a lot of information very quickly. This way, investors can see the latest prices and trade information almost as soon as it happens.

## What are the common methods used to normalize market data?

One common method to normalize market data is scaling. This means changing the numbers so they all fit on the same scale. For example, if you have stock prices from different countries in different currencies, you can convert all the prices to one currency, like US dollars. This makes it easier to compare the prices directly. Another way to scale is to use a range from 0 to 1, where the lowest price becomes 0 and the highest price becomes 1. This helps see how each price compares to the others, no matter what the original numbers were.

Another method is called standardization. This involves taking the average (mean) and the spread (standard deviation) of the data and using them to adjust the numbers. If a stock price is higher than the average, it gets a positive number after standardization. If it's lower, it gets a negative number. This way, you can see how far away each price is from the average, making it easier to spot trends and outliers. Standardization is useful when you want to understand how each piece of data relates to the whole set.

A third method is smoothing, which is used to reduce noise in the data. This means taking out small ups and downs that can make the data hard to understand. One way to smooth data is by using moving averages, where you take the average of a certain number of past data points. This helps show the general direction of the prices without getting distracted by short-term changes. Smoothing is especially helpful for seeing long-term trends and making the data clearer for analysis.

## Can you explain the process of normalizing market data with an example?

Imagine you have stock prices from two different companies, Company A and Company B. Company A's stock price is $50, and Company B's stock price is $200. If you want to compare how well these stocks are doing, it's hard to see just by looking at the raw numbers because they're on different scales. So, you decide to use a method called scaling to normalize the data. You convert both prices to a scale from 0 to 1. If the lowest price in your data set is $50 and the highest is $200, Company A's price becomes 0 (since it's the lowest) and Company B's price becomes 1 (since it's the highest). Now, you can easily see that Company A's stock is at the bottom of your scale and Company B's is at the top.

Another way to normalize the data is by using standardization. Let's say the average stock price in your data set is $125, and the standard deviation (which measures how spread out the numbers are) is $75. To standardize the prices, you subtract the average from each price and then divide by the standard deviation. For Company A, you do ($50 - $125) / $75, which equals -1. This means Company A's price is 1 standard deviation below the average. For Company B, you do ($200 - $125) / $75, which equals 1. This means Company B's price is 1 standard deviation above the average. Now, you can see how each stock's price compares to the average, making it easier to understand their performance relative to each other.

## What are the advantages of using normalized market data over raw data?

Using normalized market data makes it easier to compare different pieces of information. When you normalize data, you put everything on the same scale. This means you can look at stock prices from different countries or in different currencies and still understand how they stack up against each other. It's like having all your toys lined up neatly so you can see which ones are bigger or smaller. Without normalization, comparing raw data is like trying to compare apples to oranges; it's hard to see the real differences.

Another big advantage of normalized data is that it helps you see patterns and trends more clearly. Raw data can be messy, with lots of little ups and downs that can make it hard to understand what's really going on. When you normalize the data, you smooth out these bumps and make the big picture easier to see. This way, you can tell if a stock is going up or down over time, which helps you make better decisions about buying and selling. It's like looking at a clear map instead of a confusing one full of scribbles.

## In what scenarios would raw market data be preferred over normalized data?

Sometimes, people might choose to use raw market data instead of normalized data because they need to see the exact numbers. For example, if you're a trader making quick decisions, you need to know the exact price of a stock right now. Normalized data might smooth out these prices, which could hide important details. So, if you're trying to buy or sell at the best possible moment, raw data gives you the real numbers you need to make those fast choices.

Another time when raw data is better is when you're doing detailed research. Scientists or analysts who study markets might want to look at the raw numbers to find out why prices change the way they do. They might need to see every little up and down to understand what's going on. Normalized data can make these details less clear, so for deep research, raw data is the way to go.

## How does the choice between normalized and raw data impact data analysis?

Choosing between normalized and raw data can make a big difference in how you understand and use the information. Raw data gives you all the exact details, like the exact price of a stock at a specific time. This can be really important if you need to make quick decisions or if you're doing detailed research where you want to see every little change. Raw data lets you see the market as it really is, without any changes, which can be crucial for certain types of analysis where you need to know the precise numbers.

On the other hand, normalized data makes it easier to see the big picture and compare different things. When you normalize data, you put everything on the same scale, so you can easily see how stocks from different countries or in different currencies are doing compared to each other. This helps you spot trends and patterns more clearly because it smooths out the small ups and downs that can make raw data hard to understand. So, if you're trying to understand how things are changing over time or how different stocks stack up against each other, normalized data can be a better choice.

## What are the potential pitfalls of using normalized market data?

Using normalized market data can sometimes hide important details. When you change the numbers to fit on the same scale or smooth them out, you might miss the small changes that can be important. For example, if you're a trader who needs to buy or sell at the best moment, you need to see the exact price of a stock right now. Normalized data might not show these exact prices, which could make it harder to make quick and accurate decisions.

Another problem with normalized data is that it can be tricky to understand what the numbers really mean. When you change the data, it can be hard to know if the changes are showing you something real or if they're just because of how you changed the data. This can be confusing, especially if you're new to looking at market data. So, while normalized data can help you see big patterns and compare things easily, it's important to remember that it might not always give you the full story.

## How do different industries approach the normalization of market data?

In the finance industry, people often use normalization to make it easier to compare stocks from different countries or in different currencies. They might change all the prices to one currency, like US dollars, so they can see which stocks are doing better or worse. They also use methods like moving averages to smooth out the prices and see long-term trends. This helps them make better decisions about when to buy or sell stocks. But they have to be careful because normalizing the data can hide important details, like small changes in price that might matter a lot to traders.

In the tech industry, companies use normalization to make sense of huge amounts of data from things like website visits or app downloads. They might put all the numbers on a scale from 0 to 1 so they can compare different data sets easily. This helps them see which products are popular and how people are using them. But just like in finance, tech companies need to watch out because normalizing the data can sometimes make it hard to see what's really going on. They need to balance seeing the big picture with understanding the details.

In the healthcare industry, normalization is used to compare patient data from different places or over time. Doctors and researchers might change all the numbers to a common scale so they can see how different treatments are working. This helps them understand health trends and make better decisions about patient care. But they also need to be careful because normalizing the data can sometimes miss important details about a patient's health. They need to make sure they're not losing important information while trying to make the data easier to compare.

## What advanced techniques can be applied to enhance the normalization of complex market data sets?

One advanced technique to enhance the normalization of complex market data sets is using [machine learning](/wiki/machine-learning) algorithms. These algorithms can find patterns in the data that are hard to see with simple methods. For example, they can learn from past data to predict how prices might change in the future. This helps make the normalization process smarter because it takes into account more than just the numbers we see right now. It's like having a smart friend who can look at a lot of information and help you understand it better.

Another technique is using dimensionality reduction. This means taking a lot of different pieces of data and turning them into a smaller set that's easier to work with. For example, if you have data about stock prices, trading volumes, and company news all at once, you can use methods like Principal Component Analysis (PCA) to focus on the most important parts. This makes it easier to normalize the data because you're working with a simpler version that still captures the big picture. It's like cleaning up a messy room by sorting everything into just a few neat piles, so you can see what's important without getting overwhelmed by all the details.

## References & Further Reading

[1]: Chan, E. P. (2008). ["Quantitative Trading: How to Build Your Own Algorithmic Trading Business."](https://github.com/ftvision/quant_trading_echan_book) Wiley.

[2]: Jansen, S. (2018). ["Machine Learning for Algorithmic Trading."](https://github.com/stefan-jansen/machine-learning-for-trading) Packt Publishing.

[3]: Aronson, D. R. (2006). ["Evidence-Based Technical Analysis: Applying the Scientific Method and Statistical Inference to Trading Signals."](https://www.amazon.com/Evidence-Based-Technical-Analysis-Scientific-Statistical/dp/0470008741) Wiley.

[4]: Lopez de Prado, M. (2018). ["Advances in Financial Machine Learning."](https://www.amazon.com/Advances-Financial-Machine-Learning-Marcos/dp/1119482089) Wiley.

[5]: Bergstra, J., Bardenet, R., Bengio, Y., & Kégl, B. (2011). ["Algorithms for Hyper-Parameter Optimization."](https://dl.acm.org/doi/10.5555/2986459.2986743) Advances in Neural Information Processing Systems 24.