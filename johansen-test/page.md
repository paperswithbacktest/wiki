---
title: "Johansen test"
description: Discover the transformative role of the Johansen test in algorithmic trading. This powerful statistical tool identifies cointegration among multiple financial time series, enabling traders to uncover long-term stable relationships and optimize trading strategies. The Johansen test enhances pairs trading by pinpointing assets that move together over time, facilitating profitable mean reversion strategies. Leverage its robust methodology to elevate trading strategies and risk management in complex financial systems.
---


![Image](images/1.jpeg)

## Table of Contents

## What is the Johansen test?

The Johansen test is a statistical method used to find out if there is a long-term relationship between different sets of data. It is often used in economics to see if things like stock prices, interest rates, or other financial indicators move together over time. The test looks at several time series data and checks if they are cointegrated, which means they have a stable, long-run connection even if they might seem to move randomly in the short term.

To perform the Johansen test, you need to follow a few steps. First, you check if the data series are stationary, meaning their statistical properties do not change over time. If they are not stationary, you might need to difference the data, which means you look at the changes from one period to the next. Then, you use the Johansen test to see if there is a cointegrating relationship. The test gives you a statistic that you compare to critical values to decide if the relationship is significant. If it is, it means the series are cointegrated and have a long-term relationship.

## Why is the Johansen test used in econometrics?

The Johansen test is used in econometrics to find out if different sets of data have a long-term relationship. In economics, people often want to know if things like stock prices, interest rates, or other financial indicators move together over time. The Johansen test helps answer this question by checking if these data series are cointegrated. Cointegration means that even if the data might seem to move randomly in the short term, they have a stable, long-run connection.

To use the Johansen test, economists first check if the data series are stationary, which means their statistical properties do not change over time. If the data are not stationary, they might need to difference the data, which means looking at the changes from one period to the next. Then, they apply the Johansen test to see if there is a cointegrating relationship. The test gives a statistic that is compared to critical values to decide if the relationship is significant. If it is significant, it means the series are cointegrated and have a long-term relationship, which is very useful for making economic forecasts and understanding economic trends.

## What are the key assumptions behind the Johansen test?

The Johansen test works best when the data it uses follows certain rules. One big rule is that the data should be a time series, which means it's collected over time. The test also assumes that the data is normally distributed, which means the numbers should spread out in a bell-shaped curve. Another important rule is that the data should be integrated of the same order, which means they need to be made stationary in the same way, usually by differencing them.

Another key assumption is that the relationships between the data series stay the same over time. This means the long-term connections between things like stock prices or interest rates don't change a lot. The Johansen test also assumes that there are no big changes or shocks in the data that could mess up the results. If these assumptions are met, the Johansen test can help find out if different sets of data have a stable, long-term relationship.

## How does the Johansen test differ from other cointegration tests?

The Johansen test is different from other cointegration tests because it can find more than one cointegrating relationship at the same time. Other tests, like the Engle-Granger test, can only find one relationship. The Johansen test looks at all the data together and uses a method called maximum likelihood to see if there are any long-term connections between the data series. This makes it more powerful and useful when you think there might be several relationships between the data.

Another way the Johansen test is different is that it gives you more detailed information about the relationships it finds. For example, it can tell you how strong the relationships are and how they change over time. Other tests might just tell you if a relationship exists or not. The Johansen test also assumes that the data is normally distributed and that the relationships between the data stay the same over time. These assumptions help make the test more accurate but also mean it might not work well if the data doesn't follow these rules.

## What are the steps to perform a Johansen test?

To do a Johansen test, you first need to get your data ready. Make sure your data is a time series, meaning it's collected over time. Then, check if your data is stationary, which means its properties don't change over time. If it's not stationary, you'll need to difference the data, which means you look at the changes from one period to the next. This step is important because the Johansen test works best with stationary data. Once your data is ready, you can move on to the next step.

Next, you use the Johansen test to see if your data series are cointegrated, which means they have a stable, long-term relationship. The test uses a method called maximum likelihood to check for cointegration. It gives you a statistic that you compare to critical values to decide if the relationship is significant. If the statistic is bigger than the critical value, it means your data series are cointegrated. The Johansen test can find more than one cointegrating relationship, which makes it different from other tests. Once you know if your data is cointegrated, you can use this information to make better predictions and understand how different things are connected over time.

## What is the difference between the trace test and the maximum eigenvalue test in the Johansen framework?

In the Johansen test, there are two ways to check if different sets of data have a long-term relationship: the trace test and the maximum eigenvalue test. The trace test looks at all the possible cointegrating relationships at the same time. It adds up the eigenvalues, which are numbers that tell you how strong the relationships are, and compares this sum to a critical value. If the sum is bigger than the critical value, it means there is at least one cointegrating relationship in the data.

The maximum eigenvalue test, on the other hand, checks for cointegration one relationship at a time. It looks at the biggest eigenvalue and compares it to a critical value. If the biggest eigenvalue is bigger than the critical value, it means there is one cointegrating relationship. Then, you can keep checking the next biggest eigenvalues to see if there are more relationships. Both tests help you find out if your data series move together over time, but they do it in slightly different ways.

## How do you interpret the results of a Johansen test?

When you do a Johansen test, you get results from two tests: the trace test and the maximum eigenvalue test. These tests help you find out if different sets of data have a long-term relationship. The trace test looks at all possible relationships at once and gives you a number. If this number is bigger than a critical value, it means there is at least one long-term relationship in your data. The maximum eigenvalue test checks for these relationships one at a time. It looks at the biggest number and compares it to a critical value. If it's bigger, there's one long-term relationship, and you can keep checking for more.

After running the Johansen test, you need to look at the results to see how many long-term relationships there are. If both the trace test and the maximum eigenvalue test show that the numbers are bigger than the critical values, it means your data series move together over time. This is important because it can help you make better predictions about things like stock prices or interest rates. If the numbers are not bigger than the critical values, it means there's no long-term relationship, and the data might just be moving randomly.

## What are common pitfalls when applying the Johansen test?

One common pitfall when using the Johansen test is not checking if the data is stationary first. The test works best with data that doesn't change its properties over time. If the data isn't stationary, you need to make it so by differencing it, which means looking at the changes from one period to the next. If you skip this step, your results might not be accurate. Another mistake is assuming the data follows a normal distribution when it doesn't. The Johansen test assumes the numbers are spread out in a bell-shaped curve, so if they aren't, the test might give you wrong answers.

Another issue is not considering the possibility of structural breaks in the data. These are big changes or shocks that can mess up the long-term relationships the test is looking for. If there are structural breaks and you don't account for them, your results could be misleading. Also, it's easy to misinterpret the results of the Johansen test. Both the trace test and the maximum eigenvalue test give you numbers that you compare to critical values. If you don't understand what these numbers mean, you might think there's a long-term relationship when there isn't, or miss one that's there.

## Can you explain the mathematical formulation of the Johansen test?

The Johansen test uses math to see if different sets of data have a long-term relationship. It starts by making a big equation called a vector autoregression (VAR) model. This model looks at how each data series depends on past values of itself and other data series. Then, the test changes this VAR model into another kind of model called a vector error correction model (VECM). The VECM helps find out if the data series move together over time. The Johansen test uses something called eigenvalues, which are numbers that tell you how strong the relationships are between the data series. It compares these eigenvalues to critical values to see if the relationships are significant.

There are two ways to check for these long-term relationships in the Johansen test: the trace test and the maximum eigenvalue test. The trace test adds up all the eigenvalues and compares this sum to a critical value. If the sum is bigger than the critical value, it means there is at least one long-term relationship in the data. The maximum eigenvalue test looks at the biggest eigenvalue and compares it to a critical value. If the biggest eigenvalue is bigger than the critical value, it means there is one long-term relationship. You can keep checking the next biggest eigenvalues to see if there are more relationships. Both tests help you find out if your data series move together over time, but they do it in slightly different ways.

## How does the choice of lag length affect the Johansen test results?

The choice of lag length in the Johansen test is really important because it can change the results. Lag length is how many past time periods you look at when you're trying to see if different sets of data have a long-term relationship. If you pick a lag length that's too short, you might miss some important information about how the data series move together. On the other hand, if you pick a lag length that's too long, you might end up including too much information, which can make the test less accurate and harder to understand.

To find the right lag length, you can use different ways like information criteria, such as the Akaike Information Criterion (AIC) or the Bayesian Information Criterion (BIC). These help you choose a lag length that gives you the best balance between including enough information and keeping the model simple. Getting the lag length right is key because it affects how well the Johansen test can find long-term relationships in your data. If you choose the wrong lag length, you might think there's a long-term relationship when there isn't, or miss one that's actually there.

## What are some advanced techniques or modifications to the Johansen test?

One advanced technique for the Johansen test is to use something called the Johansen's test with structural breaks. This is useful when there are big changes or shocks in the data that could mess up the long-term relationships the test is looking for. By including these structural breaks in the test, you can get more accurate results. Another modification is to use the Johansen test with what's called a bootstrap method. This method helps you check if the results of the test are reliable by running the test many times with different sets of data that are similar to your original data. This can give you a better idea of how strong the long-term relationships really are.

Another advanced technique is to use the Johansen test with something called a regime-switching model. This is helpful when the relationships between the data series change over time, like during different economic conditions. By using a regime-switching model, you can see how the long-term relationships change from one situation to another. Also, you can use the Johansen test with what's called a panel data approach. This means you can test for long-term relationships across different groups or countries at the same time. This can give you a bigger picture of how things are connected over time and across different places.

## How can the Johansen test be implemented in statistical software like R or Python?

In R, you can use the `urca` package to do the Johansen test. First, you need to install and load the package. Then, you make your data into a time series object. After that, you use the `ca.jo` function to run the Johansen test. This function needs you to tell it the data, the type of test you want to do (like "trace" or "eigen"), and how many past time periods you want to look at, which is called the lag length. Once you run the test, you can look at the results to see if there are any long-term relationships in your data. The results will show you numbers from the trace test and the maximum eigenvalue test, which you compare to critical values to decide if the relationships are significant.

In Python, you can use the `statsmodels` library to do the Johansen test. First, you need to import the right part of the library, which is `statsmodels.tsa.vector_ar.vecm`. Then, you put your data into a format that the library can use, like a pandas DataFrame. After that, you use the `coint_johansen` function to run the Johansen test. This function needs you to give it the data, tell it how many past time periods to look at (the lag length), and what kind of test you want to do (like "trace" or "eigen"). Once you run the test, you can look at the results to see if there are any long-term relationships in your data. The results will show you numbers from the trace test and the maximum eigenvalue test, which you compare to critical values to decide if the relationships are significant.

## What is the Johansen Test and how does it work?

The Johansen test is a statistical approach used to determine the presence of cointegration among multiple I(1) time series. Recognized for its robustness in econometric analysis, the Johansen test is particularly valuable in financial markets, where understanding the long-term equilibrium relationships among assets is crucial.

Unlike the Engle-Granger test, which is only applicable to two time series and relies on a single-equation approach, the Johansen test can handle multiple time series simultaneously within a multivariate framework. This ability to simultaneously test for multiple cointegrating relationships is one of the significant improvements over the Engle-Granger test. Moreover, while the Engle-Granger method follows a two-step process that first tests for unit roots and then tests for cointegration, the Johansen method tests these within the same framework, thus potentially offering more accurate results.

The Johansen test has two main types: the trace test and the maximum eigenvalue test. Both are based on the eigenvalues of the matrix involved in the Vector Error Correction Model (VECM).

1. **Trace Test:** The trace test examines the null hypothesis that the number of cointegrating vectors is less than or equal to $r$ against the alternative of more than $r$ cointegrating vectors. The test statistic is given by:
$$
   \text{Trace statistic} = -T \sum_{i=r+1}^{n} \ln(1-\lambda_i)

$$

   where $\lambda_i$ are the estimated eigenvalues and $T$ is the sample size.

2. **Maximum Eigenvalue Test:** Conversely, the maximum eigenvalue test assesses the null hypothesis that the number of cointegrating vectors is $r$ against the alternative of $r+1$. It focuses on the largest eigenvalue using the following test statistic:
$$
   \text{Maximum eigenvalue statistic} = -T \ln(1-\lambda_{r+1})

$$

These tests allow traders and economists to test the hypothesis concerning the number of cointegrating relationships in a more nuanced fashion than earlier methods.

Through the application of the Johansen test, one can establish a deeper understanding of the dynamic relationships among financial time series, providing an essential tool for statistical [arbitrage](/wiki/arbitrage) and risk management in complex financial systems.

## What are the technical details of the Johansen Test?

The Johansen test is a robust statistical method used to determine the cointegration relationships among multiple time series variables, specifically those that are integrated of order one, denoted as I(1). This test is particularly valuable in financial markets for identifying long-term equilibrium relationships between assets.

Mathematically, the Johansen test involves the estimation of Vector Autoregressive (VAR) models. A VAR model of order $p$ for time series data $\mathbf{y}_t$ can be expressed as:

$$
\mathbf{y}_t = A_1 \mathbf{y}_{t-1} + A_2 \mathbf{y}_{t-2} + \ldots + A_p \mathbf{y}_{t-p} + \mathbf{u}_t
$$

where $\mathbf{y}_t$ is a vector of time series variables, $A_i$ are the coefficient matrices, and $\mathbf{u}_t$ is a vector of error terms.

The Johansen test uses Vector Error Correction Models (VECM), which are a restricted form of VAR for cointegrated series. It can be expressed as:

$$
\Delta \mathbf{y}_t = \Pi \mathbf{y}_{t-1} + \sum_{i=1}^{p-1} \Gamma_i \Delta \mathbf{y}_{t-i} + \mathbf{u}_t
$$

where $\Delta$ represents the first difference operator, $\Pi$ is the matrix that captures the long-run relationships among the variables, and $\Gamma_i$ captures short-run dynamics.

A crucial component of the Johansen test is determining the rank of the matrix $\Pi$. If $\Pi$ has reduced rank $r$, then there are $r$ cointegrating relationships among the variables. The test provides two [statistics](/wiki/bayesian-statistics) to test hypotheses regarding the rank of $\Pi$: the trace test and the maximum eigenvalue test.

1. **Trace Test**: This test evaluates the null hypothesis that there are at most $r$ cointegration vectors. The statistic is calculated as:

   \[ \text{Trace Statistic} = -T \sum_{i=r+1}^{N} \ln(1-\lambda_i)
$$

   where $T$ is the sample size and $\lambda_i$ are the eigenvalues.

2. **Maximum Eigenvalue Test**: This test assesses the null hypothesis that there are exactly $r$ cointegrating relationships against the alternative of $r+1$ cointegrating vectors:

   \[ \text{Max-Eigen Statistic} = -T \ln(1-\lambda_{r+1})
$$

Both tests help determine the number of cointegrating vectors, thereby identifying the long-term equilibrium relationships among the time series.

**Assumptions and Limitations**

The Johansen test assumes that the time series data is I(1) and that no structural breaks are present in the data during the sample period. The test is sensitive to the lag length of the VAR model and the assumption of linearity. Moreover, the Johansen test can be computationally intensive, especially with a large number of variables.

It is also noted that the test's power decreases when assessing cointegration relationships with small sample sizes, leading potentially to incorrect inferences about the number of cointegrating vectors. Despite these limitations, the Johansen test remains a fundamental technique for cointegration analysis in financial markets.

## References & Further Reading

[1]: Johansen, S. (1991). ["Estimation and Hypothesis Testing of Cointegration Vectors in Gaussian Vector Autoregressive Models."](https://www.econometricsociety.org/publications/econometrica/1991/11/01/estimation-and-hypothesis-testing-cointegration-vectors) Econometrica, 59(6), 1551-1580.

[2]: Lütkepohl, H. (2005). ["New Introduction to Multiple Time Series Analysis."](https://link.springer.com/book/10.1007/978-3-540-27752-1) Springer.

[3]: Alexander, C. (1999). ["Optimal Hedging Using Cointegration."](https://royalsocietypublishing.org/doi/10.1098/rsta.1999.0416) Philosophical Transactions: Mathematical, Physical and Engineering Sciences, 357(1758), 2039-2058.

[4]: Tsay, R. S. (2013). ["Multivariate Time Series Analysis: With R and Financial Applications."](https://www.semanticscholar.org/paper/Multivariate-Time-Series-Analysis%3A-With-R-and-Tsay/d4c0cfa6bf6f3a17fad19d48e98781fdc7f4174d) John Wiley & Sons.

[5]: Lopez de Prado, M. (2018). ["Advances in Financial Machine Learning."](https://www.amazon.com/Advances-Financial-Machine-Learning-Marcos/dp/1119482089) Wiley.

[6]: Chan, E. (2009). ["Quantitative Trading: How to Build Your Own Algorithmic Trading Business."](https://github.com/ftvision/quant_trading_echan_book) Wiley Trading.

[7]: Harris, R., & Sollis, R. (2003). ["Applied Time Series Modelling and Forecasting."](https://archive.org/details/appliedtimeserie0000harr) Wiley.