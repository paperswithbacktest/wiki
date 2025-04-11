---
title: "Conditional augmented Dickey-Fuller (CADF) test"
description: Explore the Conditional Augmented Dickey-Fuller (CADF) test, a key statistical tool in algorithmic trading used to assess time series stationarity. Discover how this test enhances the traditional Augmented Dickey-Fuller (ADF) by providing optimal hedge ratios essential for pairs trading. By identifying cointegrated pairs, traders can capitalize on market opportunities through mean-reversion strategies, optimizing potential returns. Understanding CADF's role in constructing more precise trading strategies can significantly improve algorithmic trading outcomes.
---


![Image](images/1.jpeg)

## Table of Contents

## What is the purpose of the Conditional augmented Dickey-Fuller (CADF) test?

The Conditional augmented Dickey-Fuller (CADF) test is used to check if two time series are cointegrated. This means it helps to see if there is a long-term relationship between them, even if they seem to move differently in the short term. The test is an extension of the regular Dickey-Fuller test, but it is more useful when we want to understand the connection between two specific series.

In simple terms, the CADF test looks at whether the difference between two series stays stable over time. If the test shows that the series are cointegrated, it means that any short-term changes will eventually balance out, and the series will move together in the long run. This is very helpful for economists and researchers who need to study how different economic factors, like prices or interest rates, interact with each other over time.

## How does the CADF test differ from the traditional Augmented Dickey-Fuller (ADF) test?

The CADF test and the traditional ADF test both help us understand time series data, but they focus on different things. The ADF test checks if a single time series is stationary, meaning its statistical properties like mean and variance don't change over time. It's useful for figuring out if we need to difference the data to make it stationary before using it in other analyses. On the other hand, the CADF test looks at the relationship between two time series to see if they are cointegrated. This means it checks if there's a stable, long-term connection between them, even if they seem to move differently in the short term.

The main difference between the two tests is their purpose. While the ADF test is used to see if one time series needs to be transformed to become stationary, the CADF test is designed to check if two time series move together in the long run. This makes the CADF test especially useful in fields like economics, where understanding the long-term relationships between different economic indicators is crucial. So, if you're looking at just one series and want to know if it's stationary, you'd use the ADF test. But if you're interested in the connection between two series over time, the CADF test is the right choice.

## What are the basic steps to perform a CADF test?

To perform a Conditional Augmented Dickey-Fuller (CADF) test, you first need to have two time series that you think might be connected in the long run. Start by running a regression of one series on the other to find the residuals. These residuals represent the difference between the two series after accounting for their relationship. Once you have the residuals, you can then apply the ADF test to these residuals instead of to the original series. This step is key because it helps you see if the residuals are stationary, which tells you if the two series are cointegrated.

After you've run the ADF test on the residuals, you'll get a test statistic and a critical value. Compare the test statistic to the critical value to decide if you should reject the null hypothesis. The null hypothesis here is that the residuals are not stationary, meaning the two series are not cointegrated. If the test statistic is more negative than the critical value, you can reject the null hypothesis and conclude that the two series are cointegrated. This means there's a long-term relationship between them, even if they seem to move differently in the short term.

## What types of data are suitable for the CADF test?

The CADF test works best with time series data that you think might be connected in the long run. This means it's good for looking at things like economic indicators, stock prices, or any other data that changes over time and might have a relationship with another series. For example, if you want to see if there's a long-term link between the price of oil and the stock price of an oil company, the CADF test can help you figure that out.

The data should be in the form of two time series that you can compare. It's important that these series are of the same length and cover the same time period. The CADF test looks at the residuals after you run a regression of one series on the other, so having complete and matching data sets is key. If your data fits these criteria, the CADF test can be a useful tool to understand if there's a stable, long-term relationship between the two series.

## How do you interpret the results of a CADF test?

When you do a CADF test, you're trying to find out if two time series have a long-term relationship. The test gives you a number called the test statistic and another number called the critical value. If the test statistic is more negative than the critical value, you can say the two series are cointegrated. This means they have a stable connection over time, even if they move differently in the short term.

If the test statistic is less negative than the critical value, you can't say the series are cointegrated. This means any short-term changes between the two series might not balance out over time. Understanding this can help you make better decisions, especially in fields like economics where knowing how different factors relate to each other is important.

## What are the common pitfalls when applying the CADF test?

One common pitfall when using the CADF test is not having enough data. The test works best with long time series because it needs a lot of data to find a stable, long-term relationship between two series. If your data set is too short, the test might not give you accurate results. Another issue is if the data doesn't cover the same time period for both series. The CADF test looks at the residuals after you run a regression of one series on the other, so having complete and matching data sets is really important.

Another thing to watch out for is not checking if the data is already stationary before you do the test. If one or both of your time series are already stationary, the CADF test might not be the right choice. It's meant for non-stationary series that might be cointegrated. Also, be careful with how you interpret the results. Just because the test says the series are cointegrated doesn't mean they will always move together in the future. It just means there's been a stable relationship in the past, and things can change.

## Can the CADF test be used for panel data, and if so, how?

The CADF test is usually used for time series data, but you can use it with panel data too. Panel data is when you have data for different groups or individuals over time. To use the CADF test with panel data, you need to look at each group or individual separately. You run the test for each one to see if their time series are cointegrated with another series. This means you'll do a lot of CADF tests, one for each group or individual in your panel data.

After you've run the tests, you can see how many of the groups or individuals show cointegration. If most of them do, it might mean there's a general long-term relationship between the two series across the whole panel. But remember, doing this many tests can make things complicated. You have to be careful about how you interpret the results because the more tests you do, the higher the chance you might find a relationship by accident. So, using the CADF test with panel data can give you useful information, but it needs to be done carefully.

## What are the statistical assumptions underlying the CADF test?

The CADF test assumes that the time series you're looking at are non-stationary. This means their statistical properties, like the mean and variance, change over time. The test also assumes that if there is a relationship between the two series, it's a linear one. This means the connection between them can be described by a straight line. Another important assumption is that the errors, or residuals, from the regression of one series on the other are normally distributed. This means the errors follow a bell-shaped curve, which is important for the test to work correctly.

Another assumption is that the time series are of the same length and cover the same time period. This is crucial because the CADF test looks at the residuals after you run a regression of one series on the other. If the data sets don't match up, the test won't give you accurate results. Finally, the test assumes that there are no structural breaks in the data. A structural break is a big change in the data that can mess up the test's results. So, it's important to check for these breaks before you do the CADF test.

## How does the choice of lag length affect the CADF test results?

The choice of lag length in the CADF test can really change the results. Lag length is how many past values you use when you're doing the test. If you pick a lag length that's too short, you might miss important patterns in the data. This can make the test say there's no long-term relationship between the two series when there actually is one. On the other hand, if you pick a lag length that's too long, you might include too much old information that's not relevant anymore. This can make the test say there is a long-term relationship when there isn't one.

Picking the right lag length is tricky but important. You can use different ways to choose it, like looking at information criteria like AIC or BIC, which help you find a good balance. If you don't choose the lag length carefully, your results might be wrong, and you could make bad decisions based on those results. So, taking the time to get the lag length right can make your CADF test more accurate and useful.

## What are some advanced modifications or extensions of the CADF test?

One advanced modification of the CADF test is the Residual-Based Bootstrap CADF test. This version uses a technique called bootstrapping to make the test more accurate. Bootstrapping is like taking many samples from your data to see how things might change. By doing this, the test can better handle situations where the data doesn't follow the usual rules, like when the errors are not normally distributed. This makes the test more reliable, especially with real-world data that can be messy and unpredictable.

Another extension is the Panel CADF test, which is used for panel data. Panel data is when you have information for different groups or individuals over time. Instead of looking at just one pair of time series, the Panel CADF test looks at many pairs at once. This can help you see if there's a general long-term relationship across all the groups or individuals. It's more complicated because you have to do the test many times, but it can give you a broader view of the relationships in your data.

## How can the CADF test be implemented in statistical software like R or Python?

In R, you can use the CADF test by using the 'urca' package. First, you need to install and load the package. Then, you run a regression of one time series on the other to get the residuals. After that, you use the 'ca.jo' function from the 'urca' package on these residuals to do the CADF test. This function gives you a test statistic and a critical value. If the test statistic is more negative than the critical value, it means the two series are cointegrated. There's a long-term relationship between them, even if they move differently in the short term.

In Python, you can use the 'statsmodels' library to do the CADF test. First, you need to import the library and then run a regression of one series on the other using the 'OLS' function to get the residuals. After that, you can use the 'adfuller' function from 'statsmodels' on these residuals to do the test. This function will give you a test statistic and a critical value. If the test statistic is more negative than the critical value, it means the two series are cointegrated. This tells you there's a stable, long-term connection between them.

## What are the recent developments or critiques of the CADF test in academic literature?

Recent developments in academic literature have focused on improving the accuracy and applicability of the CADF test. One major development is the introduction of the Residual-Based Bootstrap CADF test. This method uses a technique called bootstrapping to make the test more reliable, especially when the data doesn't follow the usual rules. Bootstrapping means taking many samples from your data to see how things might change. This helps the test handle messy real-world data better. Another development is the Panel CADF test, which is designed for panel data where you have information for different groups or individuals over time. This test looks at many pairs of time series at once to see if there's a general long-term relationship across all groups.

Critiques of the CADF test often focus on its limitations and potential pitfalls. One common critique is that the test can be sensitive to the choice of lag length. If you pick a lag length that's too short or too long, the test results might not be accurate. Another critique is that the test assumes the data is non-stationary and that the relationship between the two series is linear. If these assumptions don't hold true, the test might give you wrong results. Some researchers also point out that the CADF test can be tricky to use with panel data because it requires running the test many times, which can lead to complicated interpretations.

## What is the Augmented Dickey-Fuller (ADF) Test and how does it work?

The Augmented Dickey-Fuller (ADF) test is a statistical methodology employed to ascertain whether a given time series is stationary, with a specific focus on detecting the presence of unit roots. A time series is considered stationary when its statistical properties, such as mean and variance, remain constant over time. Detecting stationarity is crucial in time series analysis, as many statistical models assume the series to be stationary in order to make valid predictions and inferences.

At its core, the ADF test is an augmented version of the Dickey-Fuller test, designed to address some of its limitations, particularly the issue of autocorrelation in the residuals. The standard Dickey-Fuller test assesses for a unit root by estimating the following regression:

$$
\Delta y_t = \alpha + \beta t + \gamma y_{t-1} + \epsilon_t
$$

where $\Delta y_t$ is the first difference of the series $y_t$, $\alpha$ is a constant, $\beta t$ is a time trend, $\gamma$ is the coefficient of the lagged level of the series, and $\epsilon_t$ represents the error term. The null hypothesis $H_0$ posits that the series has a unit root ($\gamma = 0$), indicating non-stationarity, while the alternative hypothesis $H_1$ suggests stationarity ($\gamma < 0$).

The ADF test extends this by accounting for higher-order autoregressive processes, thus handling possible autocorrelation in the error terms. This is achieved by including lagged differences of the dependent variable:

$$
\Delta y_t = \alpha + \beta t + \gamma y_{t-1} + \sum_{i=1}^{p} \delta_i \Delta y_{t-i} + \epsilon_t
$$

In this expanded model, $\sum_{i=1}^{p} \delta_i \Delta y_{t-i}$ introduces lagged terms to capture any autocorrelated structure. The appropriate number of lags, $p$, can typically be selected using criteria such as the Akaike Information Criterion (AIC) or the Bayesian Information Criterion (BIC).

Despite its usefulness in determining stationarity, the ADF test does not directly address the requirements for constructing effective pairs trading strategies in [algorithmic trading](/wiki/algorithmic-trading). Notably, it does not provide the hedge ratio—an essential component in pairs trading—because it only focuses on single time series properties rather than relationships between multiple series. For this reason, while the ADF test serves as a fundamental stationarity check, more comprehensive tests like the Conditional Augmented Dickey-Fuller (CADF) test are required to assess cointegration and derive hedge ratios, thereby enhancing the applicability of statistical [arbitrage](/wiki/arbitrage) methods.

## What is the Real-World Application of CADF on Financial Data?

Applying the Conditional Augmented Dickey-Fuller (CADF) test to financial data enables traders to discover potential pairs trades by assessing the stationarity of spreads between two asset prices. This technique is particularly effective in identifying cointegrated securities that exhibit mean-reverting behavior over time.

One notable example is the application of the CADF test to exchange-traded funds (ETFs) like the iShares MSCI Australia [ETF](/wiki/etf-trading-strategies) (EWA) and the iShares MSCI Canada ETF (EWC). Traders use historical price data to evaluate whether these assets share a stable long-term relationship that can form the basis of a successful pairs trading strategy.

The process begins by obtaining historical price data for both EWA and EWC. Standard financial data repositories, such as Yahoo Finance, provide accessible sources for this information. The next step involves determining a potential hedge ratio and then computing the spread between the two ETFs using this ratio. The spread is defined as:

$$
\text{Spread}_t = \text{EWA}_t - \beta \times \text{EWC}_t
$$

where $\beta$ is the hedge ratio between EWA and EWC, which aims to minimize the risk of the spread.

By applying the CADF test to the computed spread, traders can ascertain whether it is stationary, which is a key criterion for effective pairs trading. A statistically significant result from the CADF test, indicating stationarity, suggests that the spread will likely revert to its mean over time, making it a candidate for profitable trading opportunities.

Practical implementation of this procedure often involves the use of computational tools and libraries. In the R programming language, libraries such as `quantmod` for accessing historical price data and `tseries` for conducting ADF and CADF tests are instrumental. Below is a simplified example, illustrating how these libraries can be utilized for a pairs trading strategy with EWA and EWC:

```r
library(quantmod)
library(tseries)

# Load historical data for EWA and EWC
getSymbols(c("EWA", "EWC"), src = "yahoo", from = "2020-01-01")

# Calculate daily returns
ewa_returns <- dailyReturn(Cl(EWA))
ewc_returns <- dailyReturn(Cl(EWC))

# Calculate the hedge ratio - for example, using linear regression
model <- lm(Cl(EWA) ~ Cl(EWC))
beta <- coef(model)[2]

# Calculate the spread
spread <- Cl(EWA) - beta * Cl(EWC)

# Apply the CADF test on the spread
adf_result <- adf.test(spread)
print(adf_result)
```

Applying this approach allowed traders to successfully identify times when the EWA and EWC diverged from their historical relationship, signaling a potential trade entry based on expected mean reversion. The empirical success of this method depends on careful attention to transaction costs and ongoing monitoring of the model's assumptions, such as the stability of the hedge ratio and market conditions.

## References & Further Reading

[1]: Engle, R. F., & Granger, C. W. J. (1987). ["Co-integration and error correction: Representation, estimation, and testing."](https://www.jstor.org/stable/1913236?read-now=1) Econometrica: Journal of the Econometric Society, 55(2), 251-276.

[2]: Banerjee, A., Dolado, J., Galbraith, J. W., & Hendry, D. F. (1993). ["Cointegration, Error Correction, and the Econometric Analysis of Non-Stationary Data."](https://academic.oup.com/book/36111) Oxford University Press.

[3]: Alexander, C. (2001). ["Market Models: A Guide to Financial Data Analysis."](https://www.casact.org/sites/default/files/old/marketmodels.pdf) John Wiley & Sons.

[4]: Tsay, R. S. (2010). ["Analysis of Financial Time Series."](https://onlinelibrary.wiley.com/doi/book/10.1002/9780470644560) John Wiley & Sons.

[5]: Harris, R. I. D. (1995). ["Using Cointegration Analysis in Econometric Modelling."](https://books.google.com/books/about/Using_Cointegration_Analysis_in_Economet.html?id=sFR0QgAACAAJ) Prentice Hall.

[6]: Chan, E. (2009). ["Quantitative Trading: How to Build Your Own Algorithmic Trading Business."](https://github.com/ftvision/quant_trading_echan_book) Wiley.