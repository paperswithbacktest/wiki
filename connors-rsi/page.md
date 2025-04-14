---
title: "Connors RSI Explained"
description: "Connors RSI Explained provides an in-depth look at a powerful technical indicator tailored for short-term trading scenarios within algorithmic trading. This article investigates into the unique enhancements Connors RSI offers over traditional RSI by integrating three key components: a short-period RSI, Up/Down Streak length, and Rate of Change function. These improvements yield a more dynamic analysis of market momentum and reversals essential for optimizing trading strategies in volatile markets. By exploring its calculation, application, and backtesting, readers will gain valuable insights into leveraging Connors RSI to enhance their trading decision-making processes."
---


![Image](images/1.jpeg)

## Table of Contents

## What is Connors RSI?

Connors RSI is a technical indicator used by traders to predict the future price movements of stocks, currencies, or other financial instruments. It was developed by Larry Connors and is a modification of the traditional Relative Strength Index (RSI). Connors RSI combines three elements: the traditional RSI, the RSI of the price change over a specific period, and the percentage of days that the price closed up over the same period. This combination aims to provide a more accurate signal of when an asset is overbought or oversold than the traditional RSI alone.

Traders use Connors RSI to make decisions about buying or selling assets. When the Connors RSI value is high, it suggests that the asset might be overbought, meaning its price may soon fall. Conversely, a low Connors RSI value indicates that the asset might be oversold, suggesting that its price could rise soon. By using these signals, traders can attempt to buy low and sell high, maximizing their potential profits. It's important for traders to use Connors RSI along with other indicators and analysis methods to increase the reliability of their trading decisions.

## Who developed Connors RSI?

Connors RSI was developed by Larry Connors. He is a well-known trader and author who wanted to make the traditional RSI better. The traditional RSI helps traders see if a stock or currency is overbought or oversold. Larry thought he could make it even more useful by combining it with other calculations.

Larry added two more parts to the traditional RSI to create Connors RSI. One part looks at how the price changes over a certain time. The other part checks how often the price ends the day higher than it started. By putting these three parts together, Connors RSI gives traders a clearer signal about when to buy or sell. This can help them make better trading decisions.

## How does Connors RSI differ from traditional RSI?

Connors RSI is different from traditional RSI because it adds two more pieces of information to the original RSI. Traditional RSI only looks at how the price of something has moved recently to see if it's overbought or oversold. But Connors RSI goes further. It includes the RSI of the price change over a certain time, which helps traders see if the price is moving up or down more quickly. It also looks at the percentage of days the price closed higher than it opened, which tells traders how often the price is going up.

These extra pieces of information make Connors RSI more detailed than traditional RSI. By combining these three parts, Connors RSI can give traders a clearer signal about when to buy or sell. This can help traders make better decisions because they have more data to look at. While traditional RSI is useful, Connors RSI tries to improve on it by giving a more complete picture of what's happening with the price.

## What are the three components of Connors RSI?

Connors RSI is made up of three parts that help traders understand if a stock or currency is overbought or oversold. The first part is the traditional RSI, which looks at how the price has moved over a short period, usually 14 days. This helps traders see if the price has gone up or down a lot recently. If the RSI is high, it might mean the price is overbought, and if it's low, it might mean the price is oversold.

The second part of Connors RSI is the RSI of the price change over a specific period, often 2 days. This part looks at how much the price has changed from one day to the next. If the price is going up quickly, this part of Connors RSI will be high, and if it's going down quickly, it will be low. This helps traders see if the price is moving in a strong direction.

The third part is the percentage of days that the price closed up over the same period, usually 200 days. This tells traders how often the price has ended the day higher than it started. A high percentage means the price has been going up more often, which could be a good sign for traders. By putting these three parts together, Connors RSI gives traders a clearer picture of what's happening with the price and helps them make better trading decisions.

## How is the first component of Connors RSI calculated?

The first component of Connors RSI is the traditional Relative Strength Index (RSI). To calculate it, you start by looking at the price changes over a certain number of days, usually 14 days. You find the average gain and the average loss over these days. The average gain is the total of all the positive price changes divided by the number of days. The average loss is the total of all the negative price changes divided by the number of days. Then, you use these averages to find the Relative Strength (RS), which is the average gain divided by the average loss.

Once you have the Relative Strength, you can calculate the RSI. The formula for RSI is 100 minus (100 divided by 1 plus RS). This gives you a number between 0 and 100. If the RSI is above 70, it means the price might be overbought, and if it's below 30, it might be oversold. This part of Connors RSI helps traders see if the price has moved a lot recently and if it might be time to buy or sell.

## How is the second component of Connors RSI calculated?

The second component of Connors RSI is the RSI of the price change over a specific period, usually 2 days. To calculate this, you look at how the price changes from one day to the next. You take the difference between the closing price of today and the closing price of yesterday. If the price went up, you have a positive number, and if it went down, you have a negative number. You do this for the last two days to see how the price has moved recently.

Then, you use these price changes to calculate the RSI for these two days. You find the average gain and the average loss over these two days. The average gain is the total of the positive changes divided by 2, and the average loss is the total of the negative changes divided by 2. You then use these averages to find the Relative Strength (RS), which is the average gain divided by the average loss. Finally, you calculate the RSI using the formula: 100 minus (100 divided by 1 plus RS). This gives you a number between 0 and 100 that shows if the price has been moving up or down quickly over the last two days.

## How is the third component of Connors RSI calculated?

The third component of Connors RSI is the percentage of days that the price closed up over a specific period, usually 200 days. To calculate this, you look at the closing price of each day and see if it's higher than the opening price. You count how many days the price closed higher than it opened. Then, you divide the number of days the price closed up by the total number of days you're looking at, which is 200 days, and multiply by 100 to get a percentage.

This percentage tells you how often the price has been going up over the last 200 days. If the percentage is high, it means the price has been closing higher than it opened more often, which could be a good sign for traders. If the percentage is low, it means the price has been closing lower than it opened more often, which might not be as good. This part of Connors RSI helps traders see the overall trend of the price over a longer period.

## How are the three components combined to form the final Connors RSI value?

The final Connors RSI value is calculated by combining the three components in a specific way. First, you take the traditional RSI over 14 days, which tells you if the price is overbought or oversold. Then, you take the RSI of the price change over the last 2 days, which shows if the price is moving up or down quickly. Finally, you calculate the percentage of days the price closed up over the last 200 days, which gives you an idea of the overall trend.

To get the final Connors RSI value, you add up these three components, but you give each one a different weight. The traditional RSI gets a weight of 1/3, the RSI of the price change gets a weight of 1/3, and the percentage of up days gets a weight of 1/3. You multiply each component by its weight and then add them all together. This gives you a number between 0 and 100, which traders use to make decisions about buying or selling.

## What are the typical thresholds used for trading signals with Connors RSI?

Traders use Connors RSI to help them decide when to buy or sell. A common threshold for a buy signal is when the Connors RSI value is below 10. This means the price might be really low and could go up soon. On the other hand, a common threshold for a sell signal is when the Connors RSI value is above 90. This means the price might be really high and could go down soon. These thresholds help traders know when it might be a good time to make a trade.

Some traders also use other numbers for their signals. For example, a buy signal might be when the Connors RSI is below 20, and a sell signal might be when it's above 80. These different thresholds can depend on what the trader thinks is best for their strategy. By using these numbers, traders try to buy when the price is low and sell when the price is high, hoping to make a profit.

## How can Connors RSI be used to identify potential buy and sell signals?

Connors RSI can help traders find good times to buy or sell by looking at certain numbers. When the Connors RSI value drops below 10, it's a sign that the price might be really low and could go up soon. This is called a buy signal. Traders see this as a chance to buy the stock or currency because they think it's a good deal and the price will rise. On the other hand, when the Connors RSI value goes above 90, it's a sign that the price might be really high and could go down soon. This is called a sell signal. Traders might sell what they own because they think the price will drop and they want to make a profit before it does.

Some traders use different numbers for their signals. For example, they might see a buy signal when the Connors RSI is below 20, and a sell signal when it's above 80. These different numbers depend on what the trader thinks works best for their strategy. By using these signals, traders try to buy when the price is low and sell when the price is high, hoping to make money. It's important for traders to use Connors RSI along with other tools and information to make the best decisions.

## What are the advantages of using Connors RSI over traditional RSI?

Connors RSI has some big advantages over the traditional RSI. One of the main advantages is that it looks at more things than just the price. Connors RSI combines the traditional RSI with how fast the price is moving and how often the price goes up. This gives traders a more complete picture of what's happening with the price. It helps them see if the price is moving in a strong direction and if it's going up more often, which can make their trading decisions more accurate.

Another advantage is that Connors RSI can give clearer signals about when to buy or sell. The traditional RSI might say a stock is overbought or oversold, but Connors RSI uses more information to decide this. By looking at the price changes over a short time and the trend over a longer time, Connors RSI can help traders spot better times to buy low and sell high. This can lead to more successful trades and help traders make more money.

## What are some advanced strategies for using Connors RSI in trading?

One advanced strategy for using Connors RSI in trading is to combine it with other technical indicators. Traders might use Connors RSI along with moving averages or Bollinger Bands to get a better idea of when to buy or sell. For example, if Connors RSI shows a buy signal and the price is also below a moving average, it might be a good time to buy. This can help traders confirm their signals and make more confident decisions. By using multiple indicators, traders can reduce the chance of making a bad trade based on a single signal.

Another strategy is to use Connors RSI for different time frames. Traders might look at Connors RSI on a daily chart and also on a shorter time frame like a 1-hour chart. If Connors RSI shows a buy signal on both time frames, it can be a stronger sign that it's a good time to buy. This can help traders find the best entry and [exit](/wiki/exit-strategy) points for their trades. By looking at different time frames, traders can get a better understanding of the overall trend and short-term movements, which can lead to better trading decisions.

## How do you calculate Connors RSI?

Calculating Connors RSI involves combining three distinct components that enhance the traditional RSI by providing a more comprehensive view of short-term market movements. These components include the Simple 3-period RSI, the Up/Down Streak with 2-period RSI, and the Rate-of-Change. Each of these elements is calculated separately and then input into the Connors RSI formula to yield the final value.

### Simple 3-period RSI

The Relative Strength Index (RSI) is a [momentum](/wiki/momentum) oscillator that measures the speed and change of price movements. The traditional formula for RSI is:

$$
\text{RSI} = 100 - \left( \frac{100}{1 + \frac{\text{Average Gain}}{\text{Average Loss}}} \right)
$$

For the Connors RSI, a 3-period RSI is specifically used, which requires calculating average gains and losses over a 3-time-period window:

1. Calculate the changes in price (today’s close - yesterday’s close) over the last 3 days.
2. Separate these into gains and losses.
3. Compute the average of gains and average of losses.
4. Substitute the values into the RSI formula.

### Up/Down Streak with 2-period RSI

The Up/Down Streak is defined by counting the number of consecutive up or down closes. The 2-period RSI of this streak provides an additional momentum measure:

1. Determine the length of the current Up/Down streak.
2. Use this streak number as the data series for calculating the 2-period RSI.
3. Apply the RSI formula over this 2-day period to the streak length.

### Rate-of-Change (ROC)

The Rate-of-Change component measures the percentage change in price over a specified number of days. For Connors RSI, the conventional span is often used:

$$
\text{ROC} = \left( \frac{\text{Current Price} - \text{Price} \, n \, \text{days ago}}{\text{Price} \, n \, \text{days ago}} \right) \times 100
$$

These values are often normalized or further processed to fit the scale of RSI values.

### Connors RSI Formula

Once all components have been calculated, the final Connors RSI is derived by combining these three equally weighted components, typically as their arithmetic mean:

$$
\text{Connors RSI} = \frac{\text{RSI} + \text{Streak RSI} + \text{ROC}}{3}
$$

This formula provides a numerical value that traders use to identify favorable trading conditions, reflecting a more thorough analysis of price momentum and streak dynamics than traditional RSI. By incorporating short-term shifts and price change rates, Connors RSI offers an enhanced tool for spotting potential market reversals and overbought or oversold conditions.

## What are the differences between Connors RSI and Traditional RSI?

Connors RSI and the traditional Relative Strength Index (RSI) are both pivotal in technical analysis, yet they serve slightly different roles due to their distinct structures, responsiveness, and applicability in various trading conditions. A fundamental comparison between these two indicators highlights their potential uses and limitations in market analysis.

### Responsiveness and Volatility

The traditional RSI, developed by J. Welles Wilder, is a momentum oscillator that oscillates between 0 and 100, offering insights into the speed and change of price movements. Typically, RSI measures the magnitude of recent price changes to evaluate overbought or oversold conditions in the price of a stock or other asset across a specified period, usually 14 days. Its formula is:

$$
RSI = 100 - \left( \frac{100}{1 + RS} \right)
$$

where $RS$ is the average gain of up periods during the specified time frame divided by the average loss of down periods over the same period.

Connors RSI, developed by Larry Connors, extends the RSI concept by incorporating not only the traditional RSI values but also short-term price momentum and the duration of price trends. It employs three components:

1. The traditional RSI, generally calculated over a short period (e.g., 3 days) to enhance responsiveness.
2. The Up/Down Streak, representing the number of consecutive days of positive or negative closes.
3. The Rate of Change (ROC) over a specific period, usually 100 days, to measure short-term price momentum.

Connors RSI is mathematically expressed as:

$$
\text{Connors RSI} = \frac{\text{RSI} + \text{Streak RSI} + \text{ROC RSI}}{3}
$$

This formula suggests Connors RSI can respond more rapidly to short-term price movements compared to traditional RSI, making it potentially more useful in volatile or fast-paced markets.

### Appropriate Application Scenarios

**Traditional RSI** is well-suited for traders interested in general market conditions over extended periods. Its traditional 14-day period provides a broader view of medium-term trends, making it ideal for longer-term trading strategies and for identifying more sustained overbought or oversold conditions.

**Connors RSI**, on the other hand, can be particularly advantageous in short-term trading scenarios due to its incorporation of multiple indicators that enhance its sensitivity to recent price movements. This makes it a valuable tool for day traders or those utilizing high-frequency trading strategies who require more immediate feedback on market momentum shifts.

### Advantages and Potential Limitations

**Advantages of Connors RSI:**
- **Enhanced Sensitivity:** By integrating additional components, Connors RSI offers a more nuanced view of price action, enabling traders to identify entry and exit points more precisely in short-term trades.
- **Versatility in Volatile Markets:** Its construction allows it to adapt to varying market volatility, providing potentially more reliable signals in rapidly changing environments.

**Potential Limitations of Connors RSI:**
- **Complex Structure:** The inclusion of multiple components increases the complexity of calculations and interpretation, which might not be ideal for novice traders.
- **Short-Term Bias:** As it emphasizes short-term indicators, there may be increased likelihood of generating false signals over extended periods or in trending markets, necessitating careful validation and backtesting.

Incorporating Connors RSI into trading strategies requires a nuanced understanding of both market dynamics and the trader's specific time horizon. While it offers the potential for more responsive market analysis than traditional RSI, traders must weigh this against its increased complexity and the needs of their particular strategy.

## Question: How effective is backtesting Connors RSI in algorithmic trading?

Backtesting is a pivotal process in validating trading strategies, offering traders insights into how a strategy would have performed based on historical data. This retrospective analysis helps identify the strengths and weaknesses of a trading strategy before actual capital is risked in the market. When applied to Connors RSI, [backtesting](/wiki/backtesting) allows traders to evaluate its ability to signal profitable entry and exit points in various market conditions.

To illustrate a backtesting scenario using Connors RSI, consider its application on the S&P 500 index. The process involves gathering historical price data of the index and calculating the Connors RSI values based on this data. A typical backtesting procedure might look like this:

1. **Data Preparation**: Acquire historical price data for the S&P 500. Ensure that the dataset is comprehensive, covering a significant period to capture different market conditions (e.g., bull and bear markets).

2. **Calculate Connors RSI**: Implement the Connors RSI formula:
$$
   \text{Connors RSI} = \frac{\text{Simple 3-period RSI} + \text{2-period RSI of the Up/Down Streaks} + \text{Rate of Change (ROC)}}{3}

$$

   Ensure that each component is calculated accurately using the data over the same historical period.

3. **Strategy Development**: Develop a trading strategy using Connors RSI signals. For instance, a simple strategy could involve opening a long position when the Connors RSI is below 20 (indicating oversold conditions) and closing the position when it exceeds 70 (indicating overbought conditions).

4. **Simulation and Analysis**: Implement the strategy in a backtesting platform, simulating trades based on historical data. Analyze the results, focusing on metrics such as the total return, maximum drawdown, and win/loss ratio.

5. **Evaluation**: Interpret the results to assess the strategy's viability. Positive results might show that the strategy consistently yields returns and manages risk effectively. Conversely, a strategy that frequently results in losses or substantial drawdowns may need adjustments, such as refining entry and exit conditions or combining Connors RSI with other indicators.

For Python implementation, libraries like `pandas` for data handling and `Zipline` for backtesting can be instrumental. Here's a simplified example of how Connors RSI might be calculated:

```python
import pandas as pd

def calculate_connors_rsi(df, period_3=3, period_2=2, roc_period=100):
    # Calculate 3-period RSI
    delta = df['Close'].diff()
    gain = (delta.where(delta > 0, 0)).rolling(window=period_3).mean()
    loss = (-delta.where(delta < 0, 0)).rolling(window=period_3).mean()
    rs = gain / loss
    rsi_3 = 100 - (100 / (1 + rs))

    # Calculate Up/Down Streak and 2-period RSI
    df['Direction'] = df['Close'].diff().apply(lambda x: 1 if x > 0 else (-1 if x < 0 else 0))
    streak = df['Direction'] * pd.Series(range(1, len(df) + 1)).where(df['Direction'] != 0)
    streak_rsi = streak.rolling(window=period_2).apply(lambda x: sum(x) / (sum(abs(x))+1e-10))

    # Rate of Change
    roc = df['Close'].pct_change(periods=roc_period) * 100

    # Connors RSI
    connors_rsi = (rsi_3 + streak_rsi + roc) / 3

    return connors_rsi

# Sample DataFrame 'df' with daily closing prices
df = pd.read_csv('historical_data.csv')
df['Connors_RSI'] = calculate_connors_rsi(df)
```

Backtesting results can provide valuable insights, such as identifying the efficacy of the Connors RSI in different time frames or market environments. Insights gained from these tests enable traders to fine-tune their strategies, improving their decision-making process and enhancing overall trading performance. Traders are encouraged to not only rely on backtesting but to also continuously monitor real-time performance and adapt strategies to evolving market dynamics.

## How can Connors RSI be implemented in algo trading?

Implementing Connors RSI (CRSI) in [algorithmic trading](/wiki/algorithmic-trading) involves a series of strategic steps that consider both the computational and market-oriented aspects of trading. Below, the key steps in effectively integrating CRSI into an algorithmic trading system are outlined:

### Steps for Integrating Connors RSI

1. **Understand the CRSI Formula:**
   Connors RSI is computed using a three-component system: a short-term RSI, an Up/Down Streak with a shorter RSI, and a Rate of Change (ROC). Before implementing, ensure you understand each part and how they contribute to the composite CRSI. The formula is typically:
$$
   \text{CRSI} = \frac{\text{RSI}_{(3)}}{3} + \frac{\text{Up/Down Streak RSI}_{(2)}}{3} + \frac{\text{ROC}}{3}

$$

   - **Simple RSI (3-period)**: This is a traditional RSI calculated over a three-day period.
   - **Up/Down Streak RSI (2-period)**: It measures the RSI over the duration of consecutive up or down closes, typically over two days.
   - **Rate of Change (ROC)**: It assesses price change over the look-back period.

2. **Data Preprocessing:**
   Collect historical price data from reliable financial data providers. Ensure data integrity by cleaning and preparing the dataset, as accurate computation of CRSI depends on precise historical data. 

3. **Algorithm Design and Scripting:**
   - **Select a Programming Language**: Python is highly recommended due to its extensive libraries, ease of use, and community support. 
   - **Scripting**: Write a script to calculate the CRSI using libraries such as Pandas for data handling and NumPy for numerical computations.

   ```python
   import pandas as pd

   def calculate_crsi(data, rsi_period=3, streak_period=2, roc_period=100):
       # Calculate RSI
       delta = data['close'].diff()
       gain = (delta.where(delta > 0, 0)).rolling(rsi_period).mean()
       loss = (-delta.where(delta < 0, 0)).rolling(rsi_period).mean()
       rs = gain / loss
       rsi = 100 - (100 / (1 + rs))

       # Calculate Up/Down Streak RSI
       streaks = delta.where(delta != 0).apply(lambda x: 1 if x > 0 else -1 if x < 0 else 0).rolling(streak_period).sum()
       streak_rsi = 100 - (100 / (1 + streaks))

       # Calculate ROC
       roc = data['close'].pct_change(roc_period) * 100

       # Calculate CRSI
       crsi = (rsi + streak_rsi + roc) / 3
       data['CRSI'] = crsi

       return data
   ```

4. **Backtesting Framework:**
   Select a robust backtesting framework like Backtrader or Zipline. Backtesting is crucial for evaluating CRSI's historical performance on selected financial instruments.

5. **Model Automation:**
   Automate the trading strategy using platforms that support algorithmic trade execution, such as MetaTrader or [Interactive Brokers](/wiki/interactive-brokers-api). Key considerations include latency, execution speed, and reliability in trade execution.

6. **Risk Management and Strategy Optimization:**
   Integrate risk management protocols to mitigate losses and optimize the CRSI parameters. This optimization may involve adjusting look-back periods or sensitivity levels based on different market conditions.

### Tools and Platforms Supporting Connors RSI Implementation

- **Python Libraries**: Utilize libraries like TA-Lib for technical analysis, including CRSI calculation.
- **Backtrader**: An open-source Python framework for backtesting trading strategies, supporting CRSI.
- **QuantConnect**: A cloud-based algorithmic trading platform offering extensive support for custom indicator strategies like CRSI.
- **MetaTrader 4/5**: Offers scripting capabilities via MQL for strategy automation, including CRSI.
- **Interactive Brokers API**: Provides connectivity for automated trade execution once CRSI buy/sell signals are generated.

The incorporation of Connors RSI within an algorithmic framework allows traders to systematically approach short-term trading by harnessing refined momentum analysis, facilitating informed decision-making and enhancing trading strategy performance.

## References & Further Reading

[1]: Wilder, J. W. (1978). ["New Concepts in Technical Trading Systems."](https://archive.org/details/newconceptsintec00wild) Trend Research.

[2]: Connors, L., & Alvarez, C. (2009). ["Short Term Trading Strategies That Work."](https://www.amazon.com/Short-Term-Trading-Strategies-That/dp/0981923909) TradingMarkets Publishing Group.

[3]: Aronson, D. R. (2006). ["Evidence-Based Technical Analysis: Applying the Scientific Method and Statistical Inference to Trading Signals."](https://www.amazon.com/Evidence-Based-Technical-Analysis-Scientific-Statistical/dp/0470008741) John Wiley & Sons.

[4]: Chan, E. P. (2008). ["Quantitative Trading: How to Build Your Own Algorithmic Trading Business."](https://github.com/ftvision/quant_trading_echan_book) John Wiley & Sons.

[5]: Jansen, S. (2018). ["Machine Learning for Algorithmic Trading."](https://www.amazon.com/Hands-Machine-Learning-Algorithmic-Trading/dp/178934641X) Packt Publishing.

[6]: Lopez de Prado, M. (2018). ["Advances in Financial Machine Learning."](https://www.amazon.com/Advances-Financial-Machine-Learning-Marcos/dp/1119482089) Wiley.

[7]: Connors Research, LLC. (2012). ["The Connors RSI: A Technical Analysis Indicator Created by Connors Research."](https://www.quantifiedstrategies.com/connors-rsi/)