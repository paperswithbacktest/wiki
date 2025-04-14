---
title: "Bollinger bands"
description: Bollinger Bands are essential in algorithmic trading, facilitating predictions of market volatility and price movements. Developed by John Bollinger, they consist of an upper, lower, and middle band, the latter being a simple moving average. Traders use them to identify potential price reversals and overbought or oversold conditions. This article explains their computation and application in automated trading strategies, outlining how Python programming can aid in implementation and backtesting to improve trading decision making.
---


![Image](images/1.jpeg)

## Table of Contents

## What are Bollinger Bands?

Bollinger Bands are a tool used in trading to help understand how a stock or other financial thing is moving. They were made by a person named John Bollinger. The tool has three lines: a middle line, which is usually the average price over a certain time, and two other lines above and below it. These outer lines move further away or closer to the middle line depending on how much the price is changing. When the price is moving a lot, the outer lines are far apart. When the price is not moving much, the outer lines are close together.

Traders use Bollinger Bands to see if a stock's price might go up or down soon. If the price touches or goes outside the top line, it might mean the price is too high and could go down soon. If the price touches or goes outside the bottom line, it might mean the price is too low and could go up soon. But, Bollinger Bands are just one tool, and traders often use them with other tools to make better guesses about what might happen next with the price.

## Who invented Bollinger Bands and when?

John Bollinger invented Bollinger Bands. He came up with this idea in the early 1980s. John Bollinger is a famous person in the world of trading and finance. He wanted to create a tool that could help traders understand how prices of stocks and other things move.

Bollinger Bands became popular because they are easy to use and can help traders see when prices might change direction. They are now used all over the world by people who trade stocks, currencies, and other financial things. John Bollinger's work on Bollinger Bands has made a big impact on how people trade.

## How are Bollinger Bands calculated?

Bollinger Bands are made up of three lines: the middle line, the upper line, and the lower line. The middle line is the average price of a stock or other financial thing over a certain number of days, usually 20 days. This average is called the Simple Moving Average (SMA). To find the SMA, you add up the closing prices for the last 20 days and then divide by 20.

The upper and lower lines are calculated using something called the standard deviation, which is a way to measure how much the price changes. The upper line is the SMA plus two times the standard deviation of the prices over the same 20 days. The lower line is the SMA minus two times the standard deviation. These lines move further apart when the price changes a lot and closer together when the price doesn't change much. This helps traders see if the price is moving a lot or staying the same.

## What do the different components of Bollinger Bands represent?

The middle line of Bollinger Bands is the Simple Moving Average (SMA) of the price over a certain number of days, usually 20 days. This line shows the average price during that time. It helps traders see the general direction the price is moving, whether it's going up, down, or staying the same. The middle line is important because it acts like a balance point for the price.

The upper and lower lines of Bollinger Bands are calculated using the standard deviation of the price over the same period. The upper line is the SMA plus two times the standard deviation, and the lower line is the SMA minus two times the standard deviation. These lines show how much the price is changing. When the price moves a lot, the upper and lower lines are far apart. When the price doesn't move much, these lines are close together. Traders use these lines to see if the price might be getting too high or too low and could change direction soon.

## How can Bollinger Bands be used in trading?

Bollinger Bands can help traders make better guesses about what might happen with the price of a stock or other thing they are trading. Traders look at where the price is compared to the middle line and the upper and lower lines of the Bollinger Bands. If the price touches or goes outside the upper line, it might mean the price is too high and could go down soon. If the price touches or goes outside the lower line, it might mean the price is too low and could go up soon. Traders use this information to decide when to buy or sell.

Another way traders use Bollinger Bands is by looking at how the bands move. When the upper and lower lines are far apart, it means the price is moving a lot, and this could be a good time to trade. When the lines are close together, it means the price is not moving much, and traders might wait for a better time to trade. Bollinger Bands are just one tool, so traders often use them with other tools to make the best decisions about when to buy or sell.

## What are the common trading strategies involving Bollinger Bands?

One common strategy using Bollinger Bands is called the Bollinger Squeeze. When the upper and lower lines of the Bollinger Bands come close together, it means the price isn't moving much. Traders see this as a sign that the price might start moving a lot soon. They wait for the price to break out of the narrow band and then trade in the direction of the [breakout](/wiki/breakout-trading). If the price breaks above the upper line, traders might buy, thinking the price will keep going up. If the price breaks below the lower line, traders might sell, thinking the price will keep going down.

Another strategy is using Bollinger Bands to spot when a stock might be overbought or oversold. If the price touches or goes above the upper line, it might mean the price is too high and could go down soon. Traders might sell at this point, expecting the price to drop. If the price touches or goes below the lower line, it might mean the price is too low and could go up soon. Traders might buy at this point, expecting the price to rise. This strategy helps traders find good times to buy or sell based on where the price is compared to the Bollinger Bands.

Traders also use Bollinger Bands with other tools to make better trading decisions. For example, they might use the Relative Strength Index (RSI) along with Bollinger Bands. If the price is near the upper Bollinger Band and the RSI shows the stock is overbought, it might be a good time to sell. If the price is near the lower Bollinger Band and the RSI shows the stock is oversold, it might be a good time to buy. Using Bollinger Bands with other tools can give traders more information to make smart trading choices.

## How do you set the parameters for Bollinger Bands?

To set the parameters for Bollinger Bands, you need to decide on three main things: the period for the moving average, the number of standard deviations for the bands, and the type of moving average to use. The most common settings are a 20-day period for the moving average, 2 standard deviations for the bands, and a Simple Moving Average (SMA). These settings work well for many traders, but you can change them to fit your trading style or the specific thing you are trading.

If you want to change the settings, you might try a shorter period like 10 days or a longer period like 50 days to see how it affects the bands. You can also change the number of standard deviations to 1 or 3 to make the bands closer or further apart. Some traders use an Exponential Moving Average (EMA) instead of an SMA because it reacts faster to recent price changes. Experimenting with different settings can help you find what works best for you, but remember that changing the settings too much can make the bands less useful for predicting price movements.

## What are the limitations of using Bollinger Bands?

Bollinger Bands are a helpful tool, but they have some limits. One big problem is that they can give wrong signals. Just because the price touches the upper or lower band doesn't always mean it will change direction. Sometimes, the price can keep moving in the same direction for a while, which can trick traders into making bad trades. Also, Bollinger Bands work best in markets that are moving a lot. In markets that are not moving much, the bands can be too close together and not give clear signals.

Another limit is that Bollinger Bands are just one tool. They don't tell the whole story about what's happening with the price. Traders need to use other tools along with Bollinger Bands to make good guesses about what might happen next. If traders only use Bollinger Bands, they might miss important information that other tools could show. This is why it's important to use Bollinger Bands with other things like the Relative Strength Index or moving averages to make better trading choices.

## How can Bollinger Bands be combined with other technical indicators?

Traders often use Bollinger Bands with other tools to make better guesses about what might happen with the price. One common way is to use Bollinger Bands with the Relative Strength Index (RSI). The RSI helps traders see if a stock is overbought or oversold. If the price touches the upper Bollinger Band and the RSI is high, it might mean the price is too high and could go down soon. If the price touches the lower Bollinger Band and the RSI is low, it might mean the price is too low and could go up soon. Using both tools together can give traders more information to make smart trading choices.

Another way to use Bollinger Bands with other tools is with moving averages. Traders might use a shorter moving average, like a 10-day moving average, along with Bollinger Bands. If the shorter moving average crosses above the middle line of the Bollinger Bands, it might be a good time to buy because the price could be starting to go up. If the shorter moving average crosses below the middle line, it might be a good time to sell because the price could be starting to go down. Combining Bollinger Bands with moving averages can help traders see trends and make better decisions about when to trade.

## What are some advanced techniques for using Bollinger Bands?

One advanced way to use Bollinger Bands is by looking at the Bollinger Bandwidth. This is the difference between the upper and lower Bollinger Bands, divided by the middle line. When the Bandwidth gets very small, it means the price isn't moving much, and traders call this a Bollinger Squeeze. A Bollinger Squeeze can be a sign that the price might start moving a lot soon. Traders watch for the price to break out of the narrow band and then trade in the direction of the breakout. This technique helps traders find good times to trade when the market might be about to get more active.

Another advanced technique is using Bollinger Bands with a tool called the Keltner Channels. Keltner Channels are similar to Bollinger Bands but use the Average True Range (ATR) instead of standard deviation to set the bands. When the Bollinger Bands and Keltner Channels both show that the price is moving a lot, it can be a strong sign that the price might keep moving in that direction. Traders look for times when the price touches or goes outside both the Bollinger Bands and the Keltner Channels to find good trading opportunities. Using these two tools together can give traders more confidence in their trading decisions.

## How do Bollinger Bands perform in different market conditions?

Bollinger Bands work well in markets that are moving a lot. When the price is going up and down a lot, the upper and lower lines of the Bollinger Bands are far apart. This helps traders see when the price might be getting too high or too low and could change direction soon. For example, if the price touches the upper line, it might mean the price is too high and could go down. If the price touches the lower line, it might mean the price is too low and could go up. Traders use this information to decide when to buy or sell.

In markets that are not moving much, Bollinger Bands can be less helpful. When the price isn't changing a lot, the upper and lower lines are close together. This makes it hard for traders to see clear signs of when the price might change direction. In these quiet markets, the Bollinger Bands might give wrong signals, and traders might wait for the market to start moving more before using the bands to make trading decisions.

## What are some real-world examples of Bollinger Bands in action?

A trader named Sarah uses Bollinger Bands to trade a stock called ABC Company. One day, she notices that the price of ABC Company's stock is touching the lower Bollinger Band. She also sees that the Relative Strength Index (RSI) is showing that the stock is oversold. Sarah decides to buy the stock because she thinks it might go up soon. A few days later, the stock price does go up, and Sarah sells it for a profit. This is an example of how Bollinger Bands can help traders find good times to buy when the price is low.

Another example is a trader named Mike who uses Bollinger Bands to trade a currency pair, like the Euro against the US Dollar. Mike sees that the price of the Euro is moving a lot, and the Bollinger Bands are far apart. He waits for the price to touch the upper Bollinger Band and sees that the price is also above the Keltner Channels. Mike decides to sell the Euro because he thinks it might go down soon. A few days later, the price of the Euro does go down, and Mike buys it back at a lower price, making a profit. This shows how Bollinger Bands can help traders find good times to sell when the price is high.

## What are Bollinger Bands and how do they work?

Bollinger Bands are a technical analysis tool that consists of three components: a Simple Moving Average (SMA) and two standard deviation lines placed above and below the SMA. These components work together to offer insights into market behavior and price dynamics.

The central line of Bollinger Bands is the SMA, typically set to a 20-day moving average of the asset's price. This moving average acts as a baseline, smoothing out price fluctuations to reveal the underlying trend. The calculation of the SMA involves summing the closing prices over a specified period and dividing by the total number of days within that period.

$$
\text{SMA}_{20} = \frac{\sum_{i=1}^{20} \text{Price}_i}{20}
$$

The Upper and Lower Bands are calculated by adding and subtracting standard deviations from the SMA, respectively. Normally, the bands are set two standard deviations away from the SMA, but traders can adjust this multiplier according to their strategy.

$$
\text{Upper Band} = \text{SMA}_{20} + (2 \times \text{Standard Deviation})
$$

$$
\text{Lower Band} = \text{SMA}_{20} - (2 \times \text{Standard Deviation})
$$

The expansion and contraction of these bands are indicative of market [volatility](/wiki/volatility-trading-strategies). When the bands widen, it signals increased volatility, while narrowing bands denote decreased volatility. This property can help traders identify potential price reversal points or conditions where the market may be overbought or oversold.

John Bollinger developed this indicator in the 1980s, with the goal of providing a relative definition of high and low prices. Since its inception, Bollinger Bands have become a standard tool for market trend assessment and volatility analysis, widely adopted by traders and analysts alike. The bands' ability to adapt to market conditions makes them a versatile addition to any trading strategy.

## How do you calculate Bollinger Bands?

Bollinger Bands are a well-regarded tool in technical analysis, widely used to gauge market volatility and identify potential price movements. Calculating Bollinger Bands involves three primary components: the Middle Band, the Upper Band, and the Lower Band.

The Middle Band represents a Simple Moving Average (SMA) of the asset's price, typically calculated over 20 days. The SMA helps to smooth out price data, providing a clearer view of price trends by averaging the closing prices over the specified period. Mathematically, it is expressed as:

$$
\text{SMA} = \frac{\sum_{i=1}^{n} P_i}{n}
$$

where $P_i$ is the closing price at day $i$ and $n$ is the number of days (usually 20).

The Upper Band is set two standard deviations above the Middle Band, while the Lower Band is two standard deviations below the Middle Band. This measure captures the degree of price [dispersion](/wiki/dispersion-trading), reflecting market volatility. The formulae are:

$$
\text{Upper Band} = \text{SMA} + (k \times \sigma)
$$

$$
\text{Lower Band} = \text{SMA} - (k \times \sigma)
$$

Here, $k$ is the number of standard deviations (commonly set to 2), and $\sigma$ represents the standard deviation of the asset's price over the same period as the SMA.

Traders have the flexibility to adjust these parameters according to specific asset characteristics or trading strategies. For instance, varying the number of days in the SMA or the number of standard deviations can tailor the sensitivity of the bands to align with different trading styles or market conditions. This adaptability makes Bollinger Bands a versatile tool in the trader's arsenal, allowing them to customize the indicator to better suit their analysis and decision-making processes.

## How can Bollinger Bands be implemented in algorithmic trading?

Algorithmic trading incorporates Bollinger Bands to automate buy and sell decisions guided by predefined criteria. This approach enables traders to exploit market opportunities based on statistical analysis rather than intuition. The core idea is to leverage the volatility information provided by Bollinger Bands to set appropriate entry and [exit](/wiki/exit-strategy) points for trades.

Python is a popular programming language used in [algorithmic trading](/wiki/algorithmic-trading) due to its extensive range of libraries for data analysis and visualization. To implement a Bollinger Bands strategy in Python, traders can use libraries such as NumPy for efficient numerical computations, pandas for data manipulation, and matplotlib or Plotly for charting.

### Basic Strategy Setup
A basic algorithmic strategy using Bollinger Bands can be established by coding specific trading conditions. Here is a simplified framework for implementing such a strategy in Python:

1. **Data Retrieval and Preparation**:
   Load historical price data of the asset of interest. This typically involves using libraries like pandas to read data from CSV files or directly from financial data providers via APIs.

2. **Indicator Calculation**:
   Calculate the Bollinger Bands using the historical data. The typical calculation involves:

   - **Middle Band (MB)**: Calculated as the moving average `(MA)` of the asset. A 20-day moving average is common:
$$
     MB_t = \frac{1}{n} \sum_{i=t-n+1}^{t} P_i

$$
     where $P_i$ is the price at day $i$ and $n$ is the number of days.

   - **Upper Band (UB)** and **Lower Band (LB)**: Calculated based on standard deviation `(σ)` levels:
$$
     UB_t = MB_t + k \times \sigma_t

$$
$$
     LB_t = MB_t - k \times \sigma_t

$$
     Typically, $k = 2$.

3. **Trading Logic**:
   Develop trading signals based on the relationship between the asset's current price and the bands:

   ```python
   def generate_signals(data, upper_band, lower_band):
       data['signal'] = 0  # No position
       data['signal'][data['Close'] > upper_band] = -1  # Sell signal
       data['signal'][data['Close'] < lower_band] = 1   # Buy signal
       return data
   ```

4. **Backtesting**:
   Evaluate the strategy by applying the trading rules to historical data to simulate how the strategy would have performed. This involves calculating key performance metrics to assess viability.

5. **Execution**:
   Set up a system to execute trades in a live environment using brokerage APIs, automating the buy and sell orders based on the signals generated.

Setting up these trading strategies involves not only coding but also rigorous [backtesting](/wiki/backtesting) to ensure robustness. The strategy needs continuous monitoring and adjustment to account for changing market conditions and to incorporate improvements discovered through further research and analysis.

## How can you backtest strategies using Bollinger Bands in Python?

Backtesting is an essential part of developing a successful trading strategy, allowing traders to evaluate the effectiveness of their ideas using historical data. When deploying Bollinger Bands in algorithmic trading, backtesting helps assess how a strategy would have performed in the past, thereby providing insight into its potential future performance.

Python is a powerful tool for backtesting strategies due to its robust ecosystem of libraries, such as pandas for data manipulation and matplotlib for data visualization. To calculate Bollinger Bands in Python, traders typically use the Simple Moving Average (SMA) and standard deviation functions available within the pandas library. The Bollinger Bands are computed by setting the middle band as the 20-day SMA, with the upper and lower bands being two standard deviations above and below this SMA, respectively. Below is a basic implementation of Bollinger Bands using Python:

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

# Load historical data into a DataFrame
data = pd.read_csv('historical_data.csv', parse_dates=['Date'], index_col='Date')

# Calculate the 20-day Simple Moving Average (SMA)
data['SMA'] = data['Close'].rolling(window=20).mean()

# Calculate the standard deviation
data['STD'] = data['Close'].rolling(window=20).std()

# Calculate the Upper and Lower Bollinger Bands
data['Upper Band'] = data['SMA'] + (data['STD'] * 2)
data['Lower Band'] = data['SMA'] - (data['STD'] * 2)

# Plotting
plt.figure(figsize=(12,6))
plt.plot(data.index, data['Close'], label='Close Price')
plt.plot(data.index, data['Upper Band'], label='Upper Bollinger Band', linestyle='--')
plt.plot(data.index, data['Lower Band'], label='Lower Bollinger Band', linestyle='--')
plt.plot(data.index, data['SMA'], label='SMA', color='k', linestyle='-')
plt.fill_between(data.index, data['Upper Band'], data['Lower Band'], color='grey', alpha=0.1)
plt.title('Bollinger Bands')
plt.legend(loc='best')
plt.show()
```

After implementing Bollinger Bands, traders evaluate strategy performance using key performance metrics. Cumulative returns give a clear picture of the total return of a strategy over a specific period. Another important measure is the Sharpe Ratio, which assesses risk-adjusted return. It calculates the average return earned in excess of the risk-free rate per unit of volatility or total risk. The formula for the Sharpe Ratio is:

$$
\text{Sharpe Ratio} = \frac{E[R] - R_f}{\sigma}
$$

where $E[R]$ is the expected return, $R_f$ is the risk-free rate, and $\sigma$ is the standard deviation of the excess return. A higher Sharpe Ratio indicates better risk-adjusted performance.

By employing these methodologies, traders can test various strategies and assumptions about market behavior, refining their approaches based on the results. This data-driven method helps in designing robust trading strategies that can withstand different market conditions.

## References & Further Reading

[1]: Bollinger, J. (2001). ["Bollinger on Bollinger Bands."](https://www.amazon.com/Bollinger-Bands-John/dp/0071373683) McGraw-Hill.

[2]: Aronson, D. (2006). ["Evidence-Based Technical Analysis: Applying the Scientific Method and Statistical Inference to Trading Signals."](https://www.amazon.com/Evidence-Based-Technical-Analysis-Scientific-Statistical/dp/0470008741) Wiley.

[3]: Pring, M. J. (2014). ["Technical Analysis Explained: The Successful Investor's Guide to Spotting Investment Trends and Turning Points."](https://www.amazon.com/Technical-Analysis-Explained-Fifth-Successful/dp/0071825177) McGraw-Hill Education.

[4]: Jansen, S. (2018). ["Hands-On Machine Learning for Algorithmic Trading."](https://www.amazon.com/Hands-Machine-Learning-Algorithmic-Trading/dp/178934641X) Packt Publishing.

[5]: Chan, E. P. (2009). ["Quantitative Trading: How to Build Your Own Algorithmic Trading Business."](https://github.com/ftvision/quant_trading_echan_book) Wiley.

[6]: Lopez de Prado, M. (2018). ["Advances in Financial Machine Learning."](https://www.amazon.com/Advances-Financial-Machine-Learning-Marcos/dp/1119482089) Wiley.

[7]: Murphy, J. (1999). ["Technical Analysis of the Financial Markets: A Comprehensive Guide to Trading Methods and Applications."](https://www.amazon.com/Technical-Analysis-Financial-Markets-Comprehensive/dp/0735200661) New York Institute of Finance.