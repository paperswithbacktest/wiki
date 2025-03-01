---
title: "Renko Chart Explanation and Uses"
description: "Discover how Renko charts offer a unique way to view market trends by focusing on price changes instead of time create effective trading strategies."
---

Renko charts are a distinctive form of financial chart that represent price movements independent of time intervals, offering a unique perspective on market trends. Unlike traditional candlestick or bar charts, which plot price movements based on specific time periods, Renko charts focus solely on price changes. This is achieved through the use of "bricks," which are added to the chart only when the price moves by a pre-determined amount known as the "box size." This methodology allows traders to filter out market noise and concentrate on significant price movements, thus simplifying the interpretation of trends and patterns.

The relevance of Renko charts in technical analysis and algorithmic trading is undeniable. By excluding the dimension of time and focusing purely on price changes, Renko charts provide a clearer picture of support and resistance levels, enhancing trend identification. This characteristic makes them highly advantageous for traders looking to identify breakouts or continuations. Additionally, in algorithmic trading, Renko charts can be integrated into trading systems to develop robust strategies that are less susceptible to the whipsaws commonly encountered in volatile markets.

![Image](images/1.jpeg)

The purpose of this article is to bridge the theoretical understanding of Renko charts with practical applications for traders. By exploring the foundational aspects of Renko charts, their integration into technical analysis, and their role in algorithmic trading, this article aims to equip traders with the knowledge needed to effectively incorporate Renko charts into their trading workflows. We will explore various facets of Renko charts, providing insights into their advantages, challenges, and potential for enhancing trading strategies. This comprehensive guide will serve as a resource for both novice and experienced traders interested in leveraging Renko charts to improve their trading outcomes.

## Table of Contents

## Understanding Renko Charts

Renko charts are distinctive financial charting tools used for tracking price movements, known for their unique method of representation that emphasizes price action over time. Unlike traditional charting techniques such as candlestick and bar charts, which place equal emphasis on both time and price, Renko charts focus solely on price changes, disregarding time and volume. This technique simplifies visualization by forming 'bricks' in a rising or falling sequence, representing a specific price movement rather than a fixed time period.

### Historical Development

Originating from Japan, much like candlestick charts, Renko charts take their name from the Japanese word 'renga', meaning 'brick'. Historically, these charts were designed to filter out market noise, allowing traders to focus on significant price fluctuations. Over time, the method gained popularity among traders and analysts looking for straightforward and efficient tracking of price trends without the clutter typically associated with traditional time-based charts.

### Comparison with Traditional Chart Types

In terms of structure, Renko charts differ significantly from traditional candlestick and bar charts. Candlestick charts use open, high, low, and close prices to form each candle, reflecting both time and price within the predefined intervals. Bar charts share a similar approach, providing a simple line representation of price changes within the time unit. Renko charts, conversely, build a new brick only after the price moves by a predetermined amount, irrespective of time. This results in a chart that reflects pure price action, ideal for traders focused on identifying trends and [momentum](/wiki/momentum).

### Key Components of Renko Charts

The primary element of Renko charts is the 'brick'. A new brick is added to the chart only when the price of an asset moves a certain distance, known as the 'box size'. Brick colors typically denote the direction of price movement—white or green for upward movements and black or red for downward. The size of each brick represents a pre-set price change, making the choice of box size crucial for chart accuracy and utility.

#### Box Size

Determining the optimal box size is paramount for effective Renko chart analysis. A smaller box size results in more bricks and greater sensitivity to price changes, potentially adding noise. Conversely, a larger box size may overlook minor yet significant movements, ideal for a focus on larger trends. Traders can adjust the box size based on their strategies and the [volatility](/wiki/volatility-trading-strategies) of the asset being observed.

#### Brick Formation

The formation of bricks in Renko charts eliminates minor fluctuations and highlights significant trends. A new brick is created only when the closing price surpasses the top or bottom of the previous brick by the box size. For example, if the box size is set to $10, a new brick would form only when prices move $10 above the last brick. This approach ensures that Renko charts are particularly effective in highlighting support and resistance levels and filtering out market noise that can be prevalent in time-based charts.

Renko charts offer a streamlined approach to price analysis, serving as a robust tool for traders prioritizing clarity and trend recognition over the traditional dynamic of time and price interaction. By highlighting significant movements and trends, these charts assist in informed decision-making, making them an attractive choice for analysts and traders seeking an alternative to conventional chart types.

## Technical Analysis Using Renko Charts

Renko charts offer a distinct advantage in technical analysis, primarily by simplifying the visualization of trends and identifying support and resistance levels. Unlike traditional chart types, such as candlestick and bar charts, Renko charts focus solely on price movement, disregarding time and [volume](/wiki/volume-trading-strategy). This unique feature enables traders to readily identify the direction and strength of a trend.

### Advantages of Using Renko Charts in Technical Analysis

Renko charts eliminate minor price fluctuations, or market noise, that can obscure trend patterns in conventional chart types. This is achieved through their construction method, where a new brick is formed only when the price exceeds a predetermined threshold, known as the box size. This method starkly contrasts with candlestick charts, where each candle represents a fixed time period regardless of price movement.

#### Simplification of Trend Identification and Support/Resistance Levels

Renko charts excel at providing a clean and clear picture of market trends. The charts' bricks change color based on the price movement direction, allowing traders to quickly identify uptrends (series of rising bricks) or downtrends (series of falling bricks). This visual clarity aids in effective decision-making by highlighting potential entry and [exit](/wiki/exit-strategy) points without the clutter of market noise.

Support and resistance levels are essential components of technical analysis, and Renko charts make it easier to identify these levels. The simplification results from the chart's structure, which smooths out price fluctuations and focuses on significant movements. Traders can observe the horizontal consolidation areas on Renko charts that often indicate strong support or resistance zones.

#### Role in Filtering Out Market Noise

Market noise, the random price movement that can often mislead traders, is significantly reduced in Renko charts. By using a fixed box size to dictate when to add a new brick, Renko charts inherently remove smaller, less significant fluctuations, allowing traders to focus on the underlying trend. This quality is particularly beneficial in volatile markets where sudden price changes can cause confusion when using other chart types.

The box size in Renko charts can be adjusted according to the trader's strategy and the asset's volatility, providing a customizable approach to filtering noise. A larger box size will yield a smoother chart, minimizing the impact of minor price movements and emphasizing the core trend, while a smaller box size will increase chart sensitivity, capturing more price action details.

Incorporating Renko charts into technical analysis can add value by streamlining trend identification processes and improving accuracy in pinpointing critical support and resistance levels. This leads to more informed trading decisions and can enhance a trader's ability to navigate complex or volatile markets.

## Algo Trading with Renko Charts

Renko charts offer a distinctive and efficient approach to integrating [algorithmic trading](/wiki/algorithmic-trading) strategies. Their ability to simplify price movements and filter out market noise makes them an ideal tool for automated trading systems. 

### Integration of Renko Charts into Algorithmic Trading Strategies

Renko charts are incorporated into algorithmic trading by establishing rules based on the visualizations they provide. These rules are typically linked to price movements denoted by Renko bricks, allowing algorithms to react programmatically to market changes. For instance, algorithms can trigger buy signals when a certain number of consecutive white bricks (indicating price increases) appear and sell signals with consecutive red bricks (indicating price declines).

The fundamental advantage of using Renko charts here is their ability to assist in identifying trends and support/resistance levels more straightforwardly than traditional chart forms. With less noise to account for, automated strategies can more readily discern genuine market trends, enhancing decision-making accuracy.

### Dynamic Customization of Renko Charts for Optimal Trading Performance

Customization of Renko chart parameters, such as brick size, plays a crucial role in tailoring these charts for algorithmic trading. The brick size can be adjusted dynamically based on market volatility or asset-specific behaviors. For example, a Python script can be developed to calculate optimal brick sizes using historical volatility:

```python
import pandas as pd
import numpy as np

def calculate_brick_size(volatility, atr_period=14):
    return np.mean(volatility.tail(atr_period))

# Assume 'volatility' is a DataFrame column with calculated historical volatility
optimal_brick_size = calculate_brick_size(volatility)
```

The above function calculates an average of the trailing volatility to propose an appropriate brick size. Such dynamic setups allow algorithms to adjust to market conditions, optimizing entries and exits based on the behavior of the underlying asset.

### Examples of Algorithmic Strategies Involving Renko Charts

One simple yet effective Renko-based algorithmic strategy involves the use of moving averages. By implementing a crossover system where a short-term moving average crosses above a long-term moving average depicted on Renko bricks, traders can automate trend-following decisions. Here's a basic Python snippet illustrating such a strategy:

```python
def renko_moving_average_strategy(data, short_window=5, long_window=20):
    data['short_ma'] = data['close'].rolling(window=short_window).mean()
    data['long_ma'] = data['close'].rolling(window=long_window).mean()

    # Generate signals
    data['signal'] = 0
    data['signal'][short_window:] = np.where(data['short_ma'][short_window:] > data['long_ma'][short_window:], 1, -1)

    return data

# Apply the strategy to Renko data
renko_strategy_data = renko_moving_average_strategy(renko_data)
```

In this strategy, the algorithm generates a 'buy' signal when the short-term moving average surpasses the long-term one, and a 'sell' signal when the reverse occurs. Such logic is simplified by the smoother nature of Renko charts, thereby enhancing the algorithm's responsiveness to genuine market shifts.

Renko charts thus hold significant potential in automating trading strategies, providing a blend of simplicity and efficiency. By facilitating improved trend recognition and reducing erroneous signals through noise filtering, they form a valuable addition to the toolkit of any algorithmic trader seeking consistent and logical market engagement.

## Tools and Platforms for Renko Chart Trading

Renko charts have gained significant popularity due to their distinct method of presenting price data, which can help traders to identify trends and make informed decisions. Several trading platforms support Renko charts, with TradingView and MetaTrader being among the most prominent. Here is an overview of these platforms and a guide on how to effectively set up and utilize Renko charts.

### TradingView

#### Overview

TradingView is a web-based platform known for its robust charting tools and social networking features. It supports a wide range of chart types, including Renko, which makes it a preferred choice for many traders.

#### Setting Up Renko Charts on TradingView

1. **Sign Up/Log In**: Create an account on [TradingView](https://www.tradingview.com) or log in if you already have one.
2. **Select a Symbol**: Enter the ticker symbol of the asset you wish to analyze in the search bar.
3. **Open Chart**: Click on the chart button next to the asset to open a new chart window.
4. **Change Chart Type**: Click on the chart type dropdown menu located on the toolbar and select 'Renko'.
5. **Adjust Box Size**: A dialog box will appear, allowing you to set the box size. You can choose between ATR (Average True Range) for dynamic sizing or a fixed box size based on your preference.

#### Features Enhancing Renko Chart Trading on TradingView

- **Custom Indicators**: TradingView allows users to customize indicators and scripts using Pine Script, enhancing analysis with tailored signals and tools.
- **Real-Time Data**: Access to real-time data and alerts ensures traders receive timely information, crucial for executing strategies based on Renko patterns.
- **Community Insights**: Traders can publish ideas and engage with the community, offering insights and shared strategies for leveraging Renko charts.

### MetaTrader

#### Overview

MetaTrader, available in versions MT4 and MT5, is another powerful platform widely used for trading various assets, particularly [forex](/wiki/forex-system). It is equipped with extensive tools and features, including support for Renko charts through custom indicators.

#### Setting Up Renko Charts on MetaTrader

1. **Install MetaTrader**: Download MetaTrader from your broker's website if not already installed.
2. **Add Renko Indicator**: Since MetaTrader does not natively support Renko charts, you'll need to import a custom Renko indicator. This can typically be found in MetaTrader’s marketplace or external sources.
3. **Open Asset Chart**: Select the asset you are interested in and open a new chart.
4. **Apply Indicator**: Navigate to 'Insert' > 'Indicators' > 'Custom' and select the Renko indicator you’ve added.
5. **Configure Settings**: Adjust the settings to set your desired box size and other parameters provided by the Renko indicator.

#### Features Enhancing Renko Chart Trading on MetaTrader

- **Expert Advisors (EAs)**: MetaTrader’s automated trading feature allows users to create or import EAs, facilitating algorithmic strategies using Renko charts.
- **Backtesting Tools**: Traders can backtest Renko-based strategies within MetaTrader’s strategy tester, providing insights into historical performance and potential effectiveness in various market conditions.
- **Advanced Technical Analysis**: The platform offers comprehensive technical analysis tools that can be used in conjunction with Renko charts for holistic market evaluation.

### Conclusion

Both TradingView and MetaTrader offer substantial capabilities for traders looking to incorporate Renko charts into their analysis and trading strategies. With TradingView's accessible interface and community, and MetaTrader's robust automation and analysis features, traders are well-equipped to harness the benefits Renko charts provide. Catering to both manual and automated trading preferences, these platforms ensure that Renko charts can be effectively utilized to enhance decision-making and ultimately, trading performance.

## Comparing Renko Charts with Heikin Ashi Charts

Renko charts and Heikin Ashi charts are both valuable tools for traders aiming to simplify price movement interpretations, although their methodologies and applications differ significantly. Understanding these distinctions and applications is crucial for traders to leverage the optimal chart type for their strategies.

Renko charts, characterized by their use of fixed brick sizes regardless of time, focus solely on price movement. This attribute makes them highly effective in filtering market noise and identifying clear trends and support/resistance levels. Each brick represents a specific price movement, and only when this predetermined price change occurs does a new brick form. This method of charting can prove advantageous for traders primarily interested in capturing trends and reducing the distraction of minor price fluctuations. The simplicity of trend identification allows traders to make more straightforward buy and sell decisions based exclusively on significant price movements.

In contrast, Heikin Ashi charts work by averaging price data to create a smoother appearance compared to traditional candlesticks. This averaging process is helpful for highlighting long-term trends and providing a clearer picture of market momentum. The Heikin Ashi technique calculates the average using the midpoint of the open and close prices over two consecutive periods, with formulas such as:

$$

\text{Heikin Ashi Close} = \frac{\text{Open}_{current} + \text{High}_{current} + \text{Low}_{current} + \text{Close}_{current}}{4} 
$$

$$

\text{Heikin Ashi Open} = \frac{\text{Open}_{previous} + \text{Close}_{previous}}{2} 
$$

Traders often favor Heikin Ashi charts for their ability to reveal the market's general direction and diminish the impact of price spikes and whipsaws.

When choosing between Renko and Heikin Ashi charts, several considerations come into play. Renko charts are preferred when the emphasis is purely on price action and minimizing noise, making them suitable for trend-following strategies in markets with substantial price movements. They excel in scenarios where price volatility needs to be isolated from temporal fluctuations. On the other hand, Heikin Ashi charts are suitable for analyzing long-term market trends and understanding overall market sentiment by smoothing short-term fluctuations. They are particularly beneficial for swing traders seeking to identify entry and exit points aligned with broader market trends.

Ultimately, the choice between Renko and Heikin Ashi charts depends on individual trading goals, market conditions, and personal preferences for noise reduction versus trend smoothing. By understanding the specific advantages and use cases of each chart type, traders can make informed decisions and potentially enhance their trading strategies.

## Case Studies and Practical Applications

Renko charts offer unique advantages that have been leveraged successfully by traders in various market environments. This section explores real-world examples, success stories, and effective strategies for trading using Renko charts.

### Real-world Examples of Trading Strategies Using Renko Charts

Renko charts are particularly useful in trend-following strategies given their ability to filter out market noise and highlight underlying trends. A common approach when using Renko charts is to combine them with moving averages or other indicators to confirm signals.

For instance:

1. **Renko and Moving Average Strategy**: Traders often use Renko charts in conjunction with a simple moving average (SMA). This involves plotting a Renko chart of a given security and overlaying an SMA to identify buy and sell signals. A typical rule might entail buying when the Renko bricks cross above the SMA and selling when they cross below.

2. **Renko with MACD**: Integrating the Moving Average Convergence Divergence (MACD) indicator with Renko charts can provide robust signals. The strategy involves entering a trade when the MACD line crosses above the signal line in a bullish Renko trend and vice versa for bearish trends. This setup helps in riding trends with potentially higher success rates.

3. **Breakout Strategy**: Renko charts can be effective for breakout trading by identifying clear support and resistance levels. A common approach involves monitoring for a new box that breaks a previously established resistance or support level, signaling a potential breakout point.

### Success Stories and Insights from Traders Using Renko-based Strategies

Several traders have reported success by incorporating Renko charts into their strategies due to their simplicity and clarity in trend identification.

- **Case Study 1**: A swing trader reported enhanced profitability by using Renko charts paired with the Relative Strength Index (RSI) to time entry and exit points more effectively. The trader noticed that by reducing the influence of minor price fluctuations, the overall trading performance improved significantly, with a better risk-reward ratio.

- **Case Study 2**: An algorithmic trader successfully integrated Renko charts into a quantitative trading model which dynamically adjusted brick sizes based on market volatility. This adaptability allowed the trading algorithm to maintain effectiveness across different market conditions, offering an edge in both trending and sideways markets.

### Lessons Learned and Tips for Applying Renko Charts Effectively

- **Optimize Brick Size**: Selecting the appropriate brick size is crucial as it directly impacts the sensitivity of the Renko chart to price movements. Starting with a percentage-based approach where the brick size is set as a percentage of the asset's ATR (Average True Range) can provide a balanced chart.

```python
def calculate_brick_size(price_data, atr_period=14, percentage=0.5):
    # Calculate ATR
    price_data['tr'] = price_data[['high']].values - price_data[['low']].values
    atr = price_data['tr'].rolling(window=atr_period).mean()
    # Calculate brick size
    brick_size = atr * (percentage / 100)
    return brick_size[-1]  # Return the last calculated brick size for the most recent ATR
```

- **Backtesting is Key**: Implement comprehensive backtesting before applying Renko-based strategies in live markets. This helps in understanding the strategy’s potential performance under various market conditions and prevents unforeseen losses.

- **Monitor Market Conditions**: Since Renko charts are trend-following, they can perform poorly during highly volatile markets with no clear trend. Traders should be cautious and possibly reconsider strategies when faced with erratic price movements.

By adopting these approaches and understanding the insights from leading traders, incorporating Renko charts into trading strategies can become a potent tool for technical analysis and trading success.

## Challenges and Limitations

Renko charts, while invaluable for certain trading techniques, present a set of challenges and limitations that traders must address to use them effectively. A common pitfall in Renko chart trading is the determination of the appropriate box size. The box size is crucial as it dictates the price movement required to form a new brick, influencing the chart's sensitivity to price changes. Choosing a box size that is too small may render the chart as noisy as traditional candlestick or bar charts, negating one of Renko’s primary advantages—noise reduction. Conversely, a box size that is too large may oversimplify market movements, leading to delayed signals and missed opportunities.

Another limitation lies in Renko charts' potential inefficacy in certain market conditions. While these charts excel in trending markets, they may prove inadequate in sideways or highly volatile markets. During such periods, the absence of time as a [factor](/wiki/factor-investing) can cause significant price moves to be consolidated into a few bricks, obscuring important market information. This characteristic can cause traders to overlook brief but significant moves that would have been more apparent on a time-based chart.

To mitigate these challenges, traders should consider using dynamic box sizing, where the box size is adjusted based on market volatility. This approach can be implemented programmatically using Python's financial libraries. For example:

```python
import numpy as np

def calculate_dynamic_box_size(prices, window=14):
    # Use an average true range (ATR) to determine the dynamic box size
    high_low = prices['high'] - prices['low']
    high_close = np.abs(prices['high'] - prices['close'].shift())
    low_close = np.abs(prices['low'] - prices['close'].shift())

    true_range = np.maximum(high_low, high_close, low_close)
    atr = true_range.rolling(window=window).mean()

    return atr
```

This script calculates a dynamic box size using the Average True Range (ATR) over a specified window. A dynamic box size allows the Renko chart to adjust to different volatility regimes, enhancing its utility across diverse market conditions.

Lastly, integrating Renko charts with other technical analysis tools may provide additional confirmation for trade decisions. Combining Renko with indicators like moving averages, RSI, or MACD can help validate trends and potential reversals. Educating oneself on these complementary tools is essential for developing a robust trading strategy and mitigating the limitations inherent to any single analytical approach.

By recognizing and addressing the limitations of Renko charts, traders can enhance their decision-making and risk management processes, leveraging Renko's strengths while compensating for its weaknesses.

## Conclusion

Renko charts offer a distinctive approach to trading, focusing on price movement rather than time intervals. Unlike traditional charts that often induce decision fatigue with excess noise, Renko charts filter out market volatility, enabling traders to identify clear trends and support/resistance levels more effectively. This makes them a valuable tool for simplifying technical analysis, particularly in volatile markets.

For traders interested in algorithmic trading, Renko charts provide advantages in developing robust strategies due to their ability to concentrate on price action. Their integration into platforms like TradingView and MetaTrader has made setting up Renko charts straightforward, facilitating seamless incorporation into automated trading systems. By dynamically adjusting the box size, traders can optimize their strategies for different market conditions, enhancing decision-making and potentially improving trading outcomes.

As trading technology continues to evolve, the use of Renko charts in technical and algorithmic trading is likely to expand. With more traders gaining access to advanced customizations and tools, experiencing the strategic benefits of Renko charts becomes increasingly feasible. Thus, exploring Renko charts can be a worthwhile addition to any trader’s toolkit, offering potential improvements in both clarity and strategy execution.

In summary, Renko charts represent an efficient tool for trend visualization and trading strategy enhancement, particularly valuable in filtering out noise inherent in traditional chart types. Traders are encouraged to integrate these charts into their workflows to take full advantage of their strategic potential. As technology advances, the future for Renko charts in both technical and algorithmic arenas looks promising, suggesting continuing growth and innovation in their application.

## FAQs

### Addressing Common Questions Traders Might Have About Renko Charts

Renko charts, distinct from traditional chart types, can generate a number of queries for traders unfamiliar with their analytical approach. Here, we address some common questions regarding their use.

1. **What are Renko Charts and How Do They Work?**

   Renko charts are a type of chart that focuses solely on price movement, filtering out time and volume. Derived from the Japanese word "renga" meaning brick, Renko charts are composed of bricks which are placed at 45-degree angles to each other. The color of the bricks typically denotes the direction of the movement, with one color for rising prices and another for falling prices.

2. **How Do I Determine the Right Box Size for Renko Charts?**

   The box size, or brick size, is a crucial element in constructing a Renko chart, as it dictates when a new brick is added. Choosing an appropriate box size involves a balance between filtering out noise and capturing significant price movements. This can be done using fixed-value methods or Average True Range (ATR) methods:

   - **Fixed Box Size:** Select a static value based on historical price levels or personal preference. This approach works well in stable markets.

   - **ATR Method:** This dynamic method considers the market's volatility, offering a box size that adjusts with market conditions. The formula to determine box size via ATR is:
$$
   \text{Box Size} = \text{ATR} \times k

$$

   Where $k$ is a multiplier determined by the trader.

3. **How to Set Up Renko Charts on Trading Platforms?**

   Most trading platforms like TradingView and MetaTrader support Renko charts. Here’s a general guide to setting them up:

   - **On TradingView:**
     - Go to the chart of your chosen instrument.
     - Click on the “Chart Type” icon in the toolbar, then select "Renko."
     - Adjust the box size using the settings option, choosing between fixed and ATR methods.

   - **On MetaTrader:**
     - Install the Renko Chart plugin, if not available by default.
     - Open a standard chart of your desired financial instrument.
     - Apply the Renko Chart indicator and configure the brick size as per your strategy.

4. **What Are the Challenges Associated with Renko Charts in Trading?**

   Traders may encounter several challenges when using Renko charts:

   - **Setting the Right Box Size:** As discussed, choosing an appropriate box size can be difficult, especially in markets with fluctuating volatility.
   - **Missed Signals:** Due to their noise-filtering ability, Renko charts might miss smaller transient price movements.
   - **Lagging Information:** Renko charts might induce lag because bricks are only added after a complete price movement equal to the box size.

5. **Strategies to Overcome Challenges with Renko Charts?**

   - To counteract missed signals and lag, traders can use a combination of Renko charts with other technical indicators like Moving Averages or RSI to confirm trends.
   - Implement backtesting and paper trading to adjust box sizes dynamically based on changing market conditions.
   - Regularly evaluate the Renko settings and adapt to market dynamics, ensuring robustness in trading strategies.

By addressing these key aspects, traders can exploit the full potential of Renko charts, integrating them seamlessly into their trading strategies.

## References & Further Reading

[1]: Kirkpatrick II, Charles D., and Dahlquist, Julie R. ["Technical Analysis: The Complete Resource for Financial Market Technicians."](https://www.amazon.com/Technical-Analysis-Complete-Financial-Technicians/dp/0134137043) FT Press.

[2]: Pring, Martin J. ["Technical Analysis Explained: The Successful Investor's Guide to Spotting Investment Trends and Turning Points."](https://www.amazon.com/Technical-Analysis-Explained-Fifth-Successful/dp/0071825177) McGraw-Hill Education.

[3]: Murphy, John J. ["Technical Analysis of the Financial Markets: A Comprehensive Guide to Trading Methods and Applications."](https://www.amazon.com/Technical-Analysis-Financial-Markets-Comprehensive/dp/0735200661) New York Institute of Finance.

[4]: Nison, Steve. ["Japanese Candlestick Charting Techniques: A Contemporary Guide to the Ancient Investment Techniques of the Far East."](https://archive.org/details/japanesecandlest0000niso) 

[5]: Lopez de Prado, Marcos. ["Advances in Financial Machine Learning."](https://www.amazon.com/Advances-Financial-Machine-Learning-Marcos/dp/1119482089) John Wiley & Sons.

[6]: Chan, Ernest P. ["Quantitative Trading: How to Build Your Own Algorithmic Trading Business."](https://github.com/ftvision/quant_trading_echan_book) John Wiley & Sons.

[7]: Aronson, David R. ["Evidence-Based Technical Analysis: Applying the Scientific Method and Statistical Inference to Trading Signals."](https://www.amazon.com/Evidence-Based-Technical-Analysis-Scientific-Statistical/dp/0470008741) John Wiley & Sons.

[8]: Jansen, Stefan. ["Machine Learning for Algorithmic Trading."](https://github.com/stefan-jansen/machine-learning-for-trading) Packt Publishing.