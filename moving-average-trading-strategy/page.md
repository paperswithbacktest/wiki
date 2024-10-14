---
title: "Moving Average Trading Strategy Explained (Algo Trading)"
description: Explore the fundamental role of moving averages in algorithmic trading with our comprehensive guide. Understand how these statistical tools smooth out price data to reveal market trends and provide clear buy or sell signals. Learn about different types of moving averages like SMA and EMA, their applications in various trading strategies, and their integration into automated trading systems. Discover insights into backtesting, mean-reversion, and trend-following strategies, while recognizing challenges such as false signals in volatile markets. Enhance your trading strategies with informed knowledge of moving averages.
---





Algorithmic trading involves using complex algorithms to make trading decisions based on various market factors. Among these strategies, moving averages play a crucial role. Moving averages are statistical indicators that help traders filter out price noise and better understand market trends by smoothing out price data over a specific period. They are fundamental in both intraday and long-term trading strategies, providing a clear view of the underlying market direction. 

The primary function of moving averages is to create a simplified representation of price movements, thereby making it easier for traders to spot trends and generate buy or sell signals. This is achieved by calculating the average of a selected range of prices, usually closing prices, over a given timeframe. By doing so, moving averages help to eliminate short-term fluctuations, thereby highlighting the overall trend direction.

This article will systematically explore various aspects of moving averages in trading. Starting with an in-depth explanation of moving averages, the discussion will cover basic concepts like the Simple Moving Average (SMA) and the Exponential Moving Average (EMA), among others. It will then proceed to describe different types of moving averages employed in trading, comparing their applications and effectiveness. The article will also cover several trading strategies that incorporate moving averages, with insights into mean-reversion and trend-following strategies, as well as the application of moving averages as dynamic support and resistance levels.

Additionally, the importance of backtesting moving average strategies will be discussed to evaluate their historical effectiveness. The integration of moving averages into algorithmic trading systems will also be examined, illustrating how these indicators can enhance automated trading. Finally, the article will address the challenges and limitations of using moving averages, particularly concerning market efficiency and the potential for false signals in volatile markets.

Types of moving averages to be discussed include the Simple Moving Average (SMA), Exponential Moving Average (EMA), Hull Moving Average (HMA), and Linear Weighted Moving Average (LWMA), among others. Each type has its unique attributes and uses, contributing to a robust set of tools for traders aiming to develop informed trading strategies.


## Table of Contents

## What is a Moving Average?

A moving average is a widely used statistical calculation in trading and financial analysis that helps smooth out short-term fluctuations and highlight longer-term trends in data series, such as stock prices. It works by calculating the average of a set of data points (prices) over a specific time period, updating this average as new data becomes available and older data is removed.

### Basic Concepts: Simple Moving Average (SMA) and Exponential Moving Average (EMA)

The Simple Moving Average (SMA) is the most basic form of moving average. It calculates the average of a specified number of most recent prices. Mathematically, the SMA for a period $n$ is represented as:

$$
\text{SMA}_n = \frac{P_1 + P_2 + P_3 + \cdots + P_n}{n}
$$

where $P$ represents the asset's prices over a certain period.

The Exponential Moving Average (EMA) gives more weight to recent prices, which makes it more responsive to new information. The formula for EMA is more complex than SMA, as it involves a multiplier:

$$
\text{EMA}_t = \left( \frac{2}{n + 1} \right) \times (P_t - \text{EMA}_{t-1}) + \text{EMA}_{t-1}
$$

where $n$ is the span of the periods, $\text{EMA}_{t}$ is the current EMA, $\text{EMA}_{t-1}$ is the previous EMA, and $P_t$ is the current price.

### Visual Difference Between SMA and EMA

In general, the SMA tends to be smoother and reacts more slowly to price changes than the EMA. This is because the EMA places a greater emphasis on more recent data points. Thus, in a rapidly changing market, the EMA will adjust its average more quickly to reflect the current trend.

For illustration, Python can be used to generate plots that showcase these differences. Here’s a simple example:

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt

# Sample price data
prices = pd.Series([22, 24, 25, 23, 22, 26, 27, 28, 30, 31])

# Calculate SMA and EMA
sma = prices.rolling(window=3).mean()
ema = prices.ewm(span=3, adjust=False).mean()

# Plotting
plt.figure(figsize=(10, 5))
plt.plot(prices, label='Price')
plt.plot(sma, label='SMA')
plt.plot(ema, label='EMA')
plt.title('Visual Comparison: SMA vs EMA')
plt.legend(loc='best')
plt.show()
```

### Significance of Moving Averages in Trading

Moving averages are crucial in technical analysis because they serve as a basis for constructing various trading strategies and tools. They help traders identify trends, determine potential support and resistance levels, and can be used for generating trading signals. In particular, moving averages are fundamental to strategies such as the Moving Average Crossover, where a short-term moving average crosses above or below a long-term moving average, indicating a potential shift in market direction. Analyzing moving averages can assist traders in making informed decisions by filtering out market noise and focusing on the underlying movement of prices.


## Types of Moving Averages in Trading

Moving averages are pivotal tools in trading, offering a mathematical method to smooth out price data over a specific period, thereby helping traders identify trends and potential reversals. Several types of moving averages are commonly employed, each with distinct characteristics and applications. Here, we explore some of the most widely used types:

### Simple Moving Average (SMA)

The Simple Moving Average (SMA) is the most basic form of moving average. It is calculated by taking the sum of closing prices over a specific period and then dividing by the number of periods. The formula is expressed as:

$$
\text{SMA} = \frac{P_1 + P_2 + \ldots + P_n}{n}
$$

where $P$ is the closing price, and $n$ is the number of periods. The SMA is straightforward to compute and provides an unweighted mean, making it less sensitive to sudden price swings.

### Exponential Moving Average (EMA)

The Exponential Moving Average (EMA) gives more weight to recent prices, making it more responsive to new information compared to the SMA. The EMA is calculated using the following recursive formula:

$$
\text{EMA}_t = \alpha \times P_t + (1 - \alpha) \times \text{EMA}_{t-1}
$$

where $\alpha = \frac{2}{n+1}$, $P_t$ is the price at time $t$, and $n$ is the number of periods. EMAs react more quickly to price changes, which can be advantageous in fast-moving markets.

### Hull Moving Average (HMA)

The Hull Moving Average (HMA) aims to reduce the lag while maintaining smoothness. It uses a weighted approach that involves several steps, combining weighted moving averages and square roots. The process is as follows:

1. Calculate a weighted moving average (WMA) over half the period.
2. Multiply the result by 2.
3. Subtract the WMA over the full period.
4. Calculate a WMA of this result over the square root of the period.

The HMA is beneficial for its quick response to market conditions without the excessive lag.

### Linear Weighted Moving Average (LWMA)

The Linear Weighted Moving Average (LWMA) assigns a descending linear weight to each price within the moving average period. Here, the most recent prices impact the average significantly more than older prices. The LWMA is computed as follows:

$$
\text{LWMA} = \frac{(n \times P_1) + ((n-1) \times P_2) + \ldots + (1 \times P_n)}{n + (n-1) + \ldots + 1}
$$

This type is useful for detecting immediate trends and responding quickly to price changes.

### Other Moving Averages

Other variations include the Triangular Moving Average (TMA), which further smooths the data by applying a double averaging process, and the Double Exponential Moving Average (DEMA), which reduces lag more effectively than a traditional EMA by applying a smoothing function twice.

### Comparison of Uses and Effectiveness

Each moving average type has its strengths and weaknesses. The SMA provides a clear overview of long-term trends but is less responsive to quick market changes due to its equal weighting. The EMA and HMA are favored for scenarios where recent price action is a priority. HMA, in particular, shines in minimizing lag, advantageous in short-term trading. LWMA, with its skewed weighting, is excellent for detecting trends quickly and is often used in fast markets.

### Backtested Results for Moving Averages

Backtesting has shown that no single moving average consistently outperforms others across all market conditions. In trending markets, EMAs and HMAs tend to have a distinct edge due to their responsiveness, often resulting in better returns compared to SMAs and LWMAs. Conversely, in volatile or sideways markets, SMAs' stable response often reduces false signals.

In summary, selecting an appropriate moving average relies heavily on the specific market environment and trading strategy. Traders often employ multiple types to maximize the robustness of their analyses and decisions.


## Moving Average Trading Strategies

Moving average trading strategies utilize moving averages to identify potential buy or sell signals in financial markets. They are primarily categorized into two broad strategies: mean-reversion and trend-following.

### Mean-Reversion Strategies Using Moving Averages
Mean-reversion strategies are based on the concept that prices and returns eventually move back to the mean or average level. They employ moving averages to identify moments when a security is overbought or oversold. A common example is the use of a simple moving average (SMA) to determine trading signals; if a price deviates significantly from its SMA, a potential reversion to the mean might be anticipated.

**Example:** For a given asset, if the current price is significantly below its 20-day SMA, a mean-reversion strategy might predict a rise in price, suggesting a buying opportunity.

### Trend-Following Strategies and Their Applications
Trend-following strategies aim to capitalize on the continuation of an existing trend. These strategies utilize moving averages to smooth price data and identify the direction of the trend.

One popular method is using an Exponential Moving Average (EMA) to filter out noise and highlight the trend. Due to its design, the EMA reacts more quickly to price changes, making it suitable for short and mid-term trading strategies.

**Python Example:**
```python
import pandas as pd

# Calculate 20-day EMA as a trend indication
data['EMA_20'] = data['Close'].ewm(span=20, adjust=False).mean()

# Generating trading signals based on price crossover
data['Signal'] = 0
data.loc[data['Close'] > data['EMA_20'], 'Signal'] = 1  # Buy
data.loc[data['Close'] < data['EMA_20'], 'Signal'] = -1  # Sell
```

### Common Strategies Like Moving Average Crossover
A Moving Average Crossover strategy uses two different moving averages: a shorter period and a longer period. A typical setup might involve a 50-day SMA (short-term) and a 200-day SMA (long-term). A buy signal is generated when the short-term moving average crosses above the long-term moving average, indicating a bullish trend; conversely, a sell signal is generated when the short-term moving average crosses below the long-term moving average, indicating a bearish trend.

### Examples of Moving Averages as Dynamic Support and Resistance Levels
Moving averages can act as dynamic support or resistance levels. For instance, during upward trends, an asset's price might repeatedly bounce off its moving average, acting as a support level. Conversely, in a downward trend, the moving average may serve as a resistance level. 

Traders use these dynamic levels to set entry and [exit](/wiki/exit-strategy) points. When the price approaches a moving average acting as support within a bullish trend, traders might consider entering a long position. Conversely, as a resistance level within a bearish trend, it might signal a short position. 

In summary, moving average trading strategies offer various applications for traders, from identifying potential reversals to confirming ongoing trends. Understanding and effectively using these strategies can enhance trading performance in different market conditions.


## Backtesting Moving Average Strategies

Backtesting is a critical component of verifying the effectiveness of trading strategies involving moving averages. It enables traders to assess performance by simulating trades based on historical data, thereby understanding potential profitability and risks before applying strategies in live markets. This process is invaluable for identifying strengths and weaknesses in trading approaches and allows for adjustments based on empirical evidence rather than conjecture.

### Review of Backtest Results for Different Strategies

Backtest results reveal that different moving average strategies perform variably across market conditions. A common approach is the Moving Average Crossover strategy, which involves two moving averages: one short-term (e.g., 50-day) and one long-term (e.g., 200-day). When the short-term average crosses above the long-term average, it signals a buy; conversely, when it crosses below, it signals a sell. Historically, this strategy has shown effectiveness in trending markets but may produce whipsaws in sideways markets.

Another strategy involves using moving averages as dynamic support and resistance levels. Price tends to bounce off these levels, offering potential buy and sell signals. Backtesting such strategies can reveal periods of effectiveness and highlight market conditions where these strategies may underperform.

### Comparison of Short-term vs Long-term Moving Average Strategies

In comparing short-term to long-term moving average strategies, it's pivotal to consider the timeframe alignment with trading goals. Short-term moving averages, such as a 5-day or 10-day, are more responsive to price changes and can signal more frequent trades, suitable for short-term traders or scalpers. However, they may also lead to numerous false signals due to market noise.

Conversely, long-term moving averages, such as the 100-day or 200-day, provide smoother signals and are typically used by long-term investors to capture major market trends. While they generate fewer signals, these signals are often more reliable but may lag, causing missed opportunities in volatile market shifts.

### Case Studies of Successful Moving Average Strategies

Successful application of moving average strategies is often documented in case studies. For example, the "Golden Cross" on the S&P 500, where the 50-day moving average crosses above the 200-day moving average, has historically been associated with bullish market conditions. Conversely, a "Death Cross," where the 50-day moving average moves below the 200-day, has often preceded more bearish conditions.

One case study involves applying a simple moving average strategy to trade the NASDAQ 100 index. By utilizing a dual moving average crossover system, traders observed a robust positive outcome over a decade, with significant drawdowns during ephemeral market volatilities minimized by strategically optimized stop-loss orders based on [backtesting](/wiki/backtesting).

### Backtesting Scripts

The backtesting of moving average strategies can be implemented using Python, leveraging libraries such as `pandas`, `numpy`, `matplotlib`, and `[backtrader](/wiki/backtrader)`. Here is a basic idea of how such a backtest could be conducted:

```python
import backtrader as bt

class MAcrossover(bt.SignalStrategy):
    def __init__(self):
        short_ma = bt.ind.SMA(period=50)
        long_ma = bt.ind.SMA(period=200)
        self.signal_add(bt.SIGNAL_LONG, short_ma - long_ma)

strategy = MAcrossover()

if __name__ == '__main__':
    cerebro = bt.Cerebro()
    cerebro.addstrategy(MAcrossover)

    data = bt.feeds.YahooFinanceData(dataname='AAPL', fromdate='2010-01-01', todate='2020-01-01')
    cerebro.adddata(data)

    cerebro.run()
    cerebro.plot()
```

This Python code sets up a simple backtesting environment using the `backtrader` library to analyze a moving average crossover strategy on Apple Inc. (AAPL) stock data over a decade. It visually plots profits and losses, aiding in identifying successful strategy elements and any adjustments needed for optimization.


## Moving Averages in Algorithmic Trading

Moving averages hold a critical position in [algorithmic trading](/wiki/algorithmic-trading) by providing a foundation for automated decision-making processes. They are used to identify trends and generate buy or sell signals based on the calculated moving average of asset prices. This methodical approach is inherent in many trading algorithms, linking historical price data with strategic trading actions.

One of the fundamental ways moving averages are integrated into algorithmic trading platforms is through their use in strategy development and signal generation. By employing moving averages such as the Simple Moving Average (SMA) or the Exponential Moving Average (EMA), traders can automate strategies that exploit price trends. For instance, the moving average crossover strategy, where a short-term moving average crosses above or below a long-term moving average, can be programmed as a signal for initiating buy or sell orders. This approach helps in reducing emotional biases as decisions are made mechanically based on pre-defined criteria.

Algorithmic trading platforms, such as MetaTrader, NinjaTrader, and QuantConnect, provide robust environments for integrating moving averages into custom trading strategies. Consider the following Python snippet using the QuantConnect platform, which illustrates a simple moving average crossover strategy:

```python
class MovingAverageCrossover(QCAlgorithm):
    def Initialize(self):
        self.SetStartDate(2020, 1, 1)  # Set Start Date
        self.SetEndDate(2023, 1, 1)    # Set End Date
        self.SetCash(10000)            # Set Strategy Cash
        self.AddEquity("SPY", Resolution.Daily)
        self.fast = self.SMA("SPY", 10, Resolution.Daily)
        self.slow = self.SMA("SPY", 30, Resolution.Daily)

    def OnData(self, data):
        # Wait for both indicators to be ready
        if not self.fast.IsReady or not self.slow.IsReady:
            return
        
        # Strategize based on the crossover
        if self.fast.Current.Value > self.slow.Current.Value:
            if not self.Portfolio.Invested:
                self.SetHoldings("SPY", 1)
        elif self.fast.Current.Value < self.slow.Current.Value:
            if self.Portfolio.Invested:
                self.Liquidate("SPY")
```

In this example, the algorithm uses two simple moving averages: a 10-day (fast) and a 30-day (slow) to determine trading signals for the SPY [ETF](/wiki/etf-trading-strategies). When the 10-day SMA crosses above the 30-day SMA, it generates a buy signal, while a crossover to the downside triggers a sell signal.

Trading algorithms harness the power of moving averages to execute trades precisely and swiftly, a necessity in today’s fast-paced markets. However, moving averages in algorithmic trading are not without limitations. They can lag in fast markets, potentially leading to delayed signals and suboptimal trading decisions. Despite these challenges, moving averages remain an essential tool in the arsenal of algorithmic traders, aiding in the construction of systematic, rules-based strategies that benefit from historical price patterns.


## Challenges and Limitations

Market efficiency and noise are key challenges in implementing moving average strategies effectively. Efficient market hypothesis suggests that asset prices reflect all available information, making it difficult for traders to consistently outperform the market using historical price data alone. Noise, or random price movements that do not reflect underlying value changes, can lead to false signals in trading, complicating the use of moving averages.

**Potential Pitfalls of Moving Average Strategies**

Moving averages are often criticized for their susceptibility to lag, as they rely on historical price data to generate signals. This time delay can cause traders to enter or exit positions too late, particularly in volatile markets. Moreover, moving averages can be prone to whipsaw effects, where frequent buy and sell signals are triggered amid sideways market movements, leading to transaction costs without significant gains.

**Impact of Lag and False Signals in Fast Markets**

In fast-moving markets, the lag inherent in moving averages becomes more pronounced. As prices change rapidly, the moving average may not accurately reflect the current market sentiment, leading to delayed responses in trading strategies. This lag can result in missed opportunities or entry and exit points that do not align with optimal market conditions.

False signals are another challenge, particularly when markets are choppy or moving sideways. These conditions can trigger numerous trading signals based on moving average crossovers or deviations, but not all will be profitable. The noise present in fast markets can exacerbate these issues, causing a higher incidence of unprofitable trades.

**Strategies to Mitigate These Challenges**

To mitigate the challenges posed by lag and false signals, traders can employ several techniques:

1. **Adaptive Moving Averages**: These adjust the speed of the moving average based on market conditions, aiming to reduce lag in fast markets while smoothing out noise. One example is the Kaufman's Adaptive Moving Average (KAMA).

2. **Combining Multiple Indicators**: By using moving averages alongside other technical indicators like the Relative Strength Index (RSI) or Moving Average Convergence Divergence (MACD), traders can confirm signals and reduce the impact of false positives.

3. **Sensitivity Adjustments**: Traders can fine-tune the sensitivity of moving averages by adjusting the period or using exponential weighting to give more emphasis to recent data, potentially reducing lag.

4. **Machine Learning Techniques**: Implementing machine learning models that learn and adapt to market conditions can enhance moving average strategies by predicting market movements more accurately and effectively filtering out noise.

5. **Time Frame Customization**: Using multiple time frames allows traders to capture both short-term trends and long-term movements, providing a more comprehensive trading perspective.

By understanding these challenges and employing strategies to mitigate them, traders can enhance the effectiveness of moving average strategies in automated and manual trading systems.


## Conclusion and Key Takeaways

Moving averages serve as a fundamental tool in algorithmic trading by smoothing out volatile price data to reveal underlying trends. Their primary benefit lies in their ability to filter out short-term fluctuations, enabling traders to focus on longer-term market movements. This feature makes them invaluable for both novice and experienced traders seeking to develop their trading strategies.

The key findings from backtesting various moving average strategies underscore their effectiveness in different market conditions. Backtesting provides empirical evidence that moving averages can enhance decision-making by identifying potential entry and exit points in the market. Specifically, moving averages are effective in trend-following strategies, where they help to confirm the direction of the trend and reduce the impact of market noise.

When implementing moving average strategies, traders should consider factors such as the choice of moving average type (e.g., Simple Moving Average, Exponential Moving Average), the selection of appropriate time periods, and the specific market conditions. For instance, shorter moving averages may be more suitable for volatile or fast-moving markets, whereas longer moving averages are often better for more stable trends. Strategies like moving average crossovers can provide clear buy or sell signals, but traders must remain cautious of potential false signals, particularly in sideways or choppy markets.

To successfully use moving average strategies, constant testing and adaptation are crucial. Markets are dynamic, and strategies that prove successful under certain conditions may not perform well under different circumstances. Traders are encouraged to regularly backtest their approaches and adjust parameters like time frames and types of moving averages to align with current market dynamics. This continuous refinement not only improves strategy efficiency but also helps in managing risk effectively.

Ultimately, moving averages are a versatile and powerful component of trading strategies, offering clear insights into market behavior when used judiciously. By combining them with rigorous backtesting and a willingness to adapt to market shifts, traders can leverage moving averages to make more informed trading decisions.


## FAQs

### FAQs

**1. What are the most effective types of moving averages for trading?**

The effectiveness of a moving average can depend on the specific market conditions and trading goals. Simple Moving Averages (SMA) are commonly used for their smoothness and simplicity, making them suitable for identifying longer-term trends. Exponential Moving Averages (EMA), on the other hand, react more quickly to price changes and are preferred in volatile markets or when timing is more crucial. Traders often find a combination of both, such as using a short-term EMA with a long-term SMA, beneficial for crossover strategies, which trigger buy or sell signals.

**2. How does market condition affect the choice of moving average?**

Market conditions significantly impact the choice of moving averages. In trending markets, traders might prefer EMAs due to their responsiveness, allowing quicker adaptation to new trends. In contrast, SMAs are often favored in range-bound markets as they smooth out erratic price movements and help identify [breakout](/wiki/breakout-trading) points. For instance, in a highly volatile market, a shorter period EMA might be used to capture quick changes, while in a stable market, a longer SMA could be preferred for trend confirmation.

**3. How should moving averages be used with other indicators?**

To enhance the robustness of trading strategies, moving averages are often used in conjunction with other technical indicators. Combining moving averages with oscillators like the Relative Strength Index (RSI) can provide more comprehensive insights. For example, a trader might look for an RSI divergence when a moving average crossover occurs, adding a layer of confirmation before executing trades. Volume indicators are also useful; a moving average crossover accompanied by a significant [volume](/wiki/volume-trading-strategy) increase might indicate a stronger price movement.

**4. Are there any downsides to using moving averages in trading?**

While moving averages are powerful tools, they come with limitations. One primary drawback is lag, as they are based on historical prices. This lag can lead to delayed signals, which might result in entering or exiting trades later than optimal. False signals are another challenge, especially in choppy markets, where prices frequently cross the moving average without establishing a clear trend. Strategies to mitigate these include adjusting the moving average period or using additional indicators to filter signals.

**5. How can I backtest moving average strategies effectively?**

Backtesting is essential for verifying the effectiveness of moving average strategies. A good approach involves using a reliable trading platform that supports historical data testing. Traders should define clear entry and exit rules based on moving average signals and incorporate transaction costs into the model to get realistic results. Splitting historical data into training and validation sets can help measure the strategy's predictive capabilities. Analyzing metrics like total return, Sharpe ratio, and maximum drawdown will provide insights into the strategy's performance.

Here is a simple Python code snippet for backtesting a moving average crossover strategy using the pandas library:

```python
import pandas as pd

# Load historical price data
data = pd.read_csv('historical_data.csv')
data['SMA_20'] = data['Close'].rolling(window=20).mean()
data['SMA_50'] = data['Close'].rolling(window=50).mean()

# Define entry and exit signals
data['Signal'] = 0
data['Signal'][20:] = np.where(data['SMA_20'][20:] > data['SMA_50'][20:], 1, -1)

# Calculate daily returns
data['Return'] = data['Close'].pct_change()
data['Strategy_Return'] = data['Signal'].shift(1) * data['Return']

# Calculate cumulative returns
cumulative_return = (1 + data['Strategy_Return']).cumprod()
print(f"Cumulative Strategy Return: {cumulative_return.iloc[-1]}")
```

This illustrates how to code a simple strategy that buys when the shorter SMA crosses above the longer SMA, and sells otherwise. Adjustments can be made to fit different market conditions or to incorporate additional trading rules.




## References & Further Reading

[1]: [Brock, W., Lakonishok, J., & LeBaron, B. (1992). "Simple Technical Trading Rules and the Stochastic Properties of Stock Returns."](https://www.jstor.org/stable/2328994) *The Review of Financial Studies, 5*(4), 173-205. 

[2]: ["Technical Analysis of the Financial Markets: A Comprehensive Guide to Trading Methods and Applications"](https://www.amazon.com/Technical-Analysis-Financial-Markets-Comprehensive/dp/0735200661) by John J. Murphy.

[3]: [Jain, S. (2021). "Algorithmic Trading using Python: Technical and Fundamental Analysis using Python"](https://en.wikipedia.org/wiki/Diwali)

[4]: [Prado, M. L. de. (2018). "Advances in Financial Machine Learning."](https://www.amazon.com/Advances-Financial-Machine-Learning-Marcos/dp/1119482089) John Wiley & Sons.

[5]: [Chan, E. P. (2009). "Quantitative Trading: How to Build Your Own Algorithmic Trading Business."](https://github.com/ftvision/quant_trading_echan_book) John Wiley & Sons.