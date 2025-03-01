---
title: "Crush Spread Analysis"
description: "Explore agricultural futures and the impact of crush spreads in soybean processing using algorithmic trading to optimize risk management and enhance profitability."
---

Agricultural futures are a pivotal component of global markets, serving as essential instruments for agricultural commodities trading. These financial contracts obligate the buyer to purchase, and the seller to sell, a specific quantity of an agricultural product at a predetermined price and future date. They are standardized contracts traded on future exchanges and play a critical role in price discovery, risk management, and market liquidity. The agricultural sector, encompassing staple commodities like corn, wheat, soybeans, and coffee, relies heavily on futures to stabilize income and mitigate the risks associated with price volatility.

Among the various strategies employed in agricultural commodities trading, crush spreads hold significant importance, particularly in the soybean processing industry. A crush spread is a trading strategy that involves simultaneously purchasing soybean futures and selling futures of the soybean products, namely soybean meal and soybean oil. This spread is crucial for processors, as it helps manage price risks and maximize profitability by capturing the differential between the input costs (soybeans) and the output prices (meal and oil). This price differential is indicative of the gross processing margin, providing valuable insights into operational profitability.

![Image](images/1.jpeg)

Algorithmic trading has emerged as a transformative force in managing trades efficiently within commodities futures markets. It employs complex algorithms to execute trading decisions at unprecedented speeds, which are impossible through manual trading. Algorithms in this domain analyze market data, identify trading opportunities, and execute trades automatically based on predefined criteria. This technology allows traders to exploit market inefficiencies swiftly and consistently, enhancing trade execution and minimizing human error and emotional bias.

The primary purpose of this article is to elucidate the concepts and strategies associated with trading agricultural futures, focusing on the implementation of crush spreads and the integration of algorithmic trading. By comprehending these strategies, traders can effectively manage risks and optimize profitability in the dynamic landscape of agricultural futures markets.

## Table of Contents

## Understanding Agricultural Futures

Agricultural futures are standardized contracts that obligate the buyer to purchase, and the seller to deliver, a specified quantity and quality of an agricultural product at a predetermined future date and price. These contracts are traded on futures exchanges and play a crucial role in facilitating price discovery and risk management for market participants. By locking in prices today for goods delivered tomorrow, these contracts help stabilize prices and provide a hedge against future price volatility.

Soybeans, soybean oil, and soybean meal are commodities of significant importance in agricultural futures markets. Soybeans serve as a versatile crop used for various applications, including as raw material for livestock feed, cooking oil, and biofuels. Soybean oil and soybean meal, products derived from soybeans, are traded separately, each with distinct supply and demand dynamics. The interdependence of these commodities means fluctuations in the price of one can influence the others, making them pivotal for traders and processors.

Market participants in agricultural futures include a diverse array of stakeholders. Farmers and producers use futures contracts to lock in prices for their crops, thus safeguarding against adverse price movements. Processors and manufacturers, such as those in the food and beverage industry, engage in futures trading to ensure stable input costs. Speculators, including hedge funds and independent traders, participate to capitalize on price changes for profit. Additionally, institutional players like commodity funds and commercial hedgers use futures to diversify portfolios and manage risk.

The prices of agricultural futures are sensitive to global supply and demand conditions. Natural factors such as weather patterns, seasonal changes, and crop yields influence supply levels, while economic factors such as consumer preferences and global trade policies affect demand. Fluctuations in supply and demand can lead to significant price [volatility](/wiki/volatility-trading-strategies), which affects the global markets for agricultural products. For instance, droughts in major soybean-producing regions can reduce supply and trigger price spikes, impacting everything from local economies to international trade balances.

In conclusion, agricultural futures contracts are essential tools for managing risk and facilitating trade in the agricultural sector. The trading of soybeans, along with soybean oil and meal, is vital for maintaining market balance and providing stability amid fluctuating global supply and demand dynamics. Understanding these contracts allows market participants to navigate the complexities of the agricultural market and make informed trading decisions.

## What is a Crush Spread?

A crush spread is a trading strategy utilized in the agricultural commodities market, specifically targeting the soybean processing chain, involving soybeans, soybean oil, and soybean meal. This strategy is used primarily to hedge against price volatility associated with the soybean market and to enhance profit margins for processors and traders.

The crush spread derives its name from the process of "crushing" soybeans into their derivative products: soybean oil and soybean meal. Traders and processors often use this spread as a measure of profitability, reflecting the difference between the cost of raw soybeans and the combined sales value of its derived products, soybean oil and soybean meal. The basic formula for the crush spread can be represented as follows:

$$
\text{Crush Spread} = (\text{Price of Soybean Oil} \times \text{Oil Yield}) + (\text{Price of Soybean Meal} \times \text{Meal Yield}) - \text{Price of Soybeans}
$$

Typically, a standard bushel of soybeans yields approximately 11 pounds of soybean oil and 44 pounds of soybean meal. These yields are integral components in calculating the effectiveness of the crush spread.

When comparing crush spreads to other spread strategies like the crack spread in oil refining, both strategies involve converting a raw commodity into finished goods and are used to manage processing margins. However, the crush spread is unique to the agricultural sector, dealing with soybeans and their derivatives, whereas the crack spread deals with [crude oil](/wiki/crude-oil) and petroleum products such as gasoline and heating oil.

The components of the soybean crush spread consist of:

1. **Soybeans:** The raw agricultural product that undergoes processing.
2. **Soybean Oil:** One of the primary products obtained from processing soybeans, used in cooking, biodiesel, and various industrial applications.
3. **Soybean Meal:** The remaining product after oil extraction, primarily used as animal feed due to its high protein content.

Crush spreads are vital in hedging against price volatility within the soybean market. Traders and processors can mitigate the risk associated with fluctuating prices by locking in crush spread trades. This strategy protects against adverse market movements, ensuring that the processing margin remains stable. Profitability is secured by effectively balancing the input costs (soybeans) with the revenue generated from the outputs (soybean oil and soybean meal).

Moreover, by utilizing crush spreads, market participants can capitalize on opportunities presented by discrepancies between expected and actual market prices, thereby optimizing their profit margins. In an environment characterized by significant price swings, having a reliable hedging mechanism like crush spreads is crucial for maintaining financial stability and achieving consistent gains in the agricultural commodities market.

## Mechanics of Crush Spreads

Crush spreads are a vital component in agricultural futures trading, particularly within the soybean market. The crush spread strategy involves the simultaneous buying and selling of soybeans, soybean oil, and soybean meal futures contracts. This strategy allows traders to hedge against price volatility and capture profit margins from processing soybeans into its derivative products. 

### Breakdown of Crush Spreads Calculation

A crush spread is calculated using the prices of soybean futures and the futures prices of the products obtained from crushing soybeans: soybean meal and soybean oil. The formula for a basic crush spread can be given as:

$$
\text{Crush Spread} = (\text{Soybean Meal Price} \times \text{Multiplier}) + (\text{Soybean Oil Price} \times \text{Multiplier}) - (\text{Soybean Price} \times \text{Units})
$$

Here, the multipliers convert the prices of soybean meal and oil to reflect their respective yield ratios from soybean processing. These ratios are standard in the industry, typically representing the quantities obtained from crushing a bushel of soybeans.

### Gross Processing Margin

The gross processing margin (GPM) represents the difference between the cost of raw soybeans and the total value of the processed products—soybean oil and soybean meal. This margin is crucial for processing plants as it reflects their potential profitability. A higher GPM suggests a profitable opportunity for processors to capitalize on favorable price differences through crush spreads. The GPM can be succinctly expressed as:

$$
\text{GPM} = \text{Total Value of Products} - \text{Cost of Soybeans}
$$

### Executing a Long and Short Crush Spread

To execute a **long crush spread**, a trader would:
1. Buy futures on soybean meal and soybean oil.
2. Sell futures on soybeans.

This strategy profits from an increase in the margin, implying either a rise in product prices or a drop in soybean prices.

Conversely, a **short crush spread** involves:
1. Selling futures on soybean meal and soybean oil.
2. Buying futures on soybeans.

This position gains from a decrease in the margin, capturing profits when product prices fall relative to soybean costs.

### Real-World Example

Consider a scenario where the futures prices are as follows:
- Soybeans at $9.75 per bushel.
- Soybean meal at $300 per short ton.
- Soybean oil at $0.31 per pound.

For simplification, presuming a standard industry yield, from one bushel of soybeans, a processor can produce 44 pounds (0.022 short tons) of soybean meal and 11 pounds of soybean oil. Hence, the crush spread would be calculated by:

$$
\text{Crush Spread} = (300 \times 0.022) + (0.31 \times 11) - (9.75)
$$

Calculating this:

$$
\text{Soybean Meal Value} = 300 \times 0.022 = 6.6
$$
$$
\text{Soybean Oil Value} = 0.31 \times 11 = 3.41
$$
$$
\text{Total Product Value} = 6.6 + 3.41 = 10.01
$$
$$
\text{Crush Spread} = 10.01 - 9.75 = 0.26
$$

A positive crush spread of $0.26 indicates a profitable opportunity from processing soybeans into its derivatives. Understanding and calculating these spreads allow traders and processors to manage price risks effectively, ultimately maximizing their profitability in a volatile market.

## Algorithmic Trading in Commodities Futures

Algorithmic trading in commodities futures involves the use of computer programs to automate the trading process, allowing for rapid execution of trades based on predefined criteria. This approach offers several benefits in the commodities market. Firstly, [algorithmic trading](/wiki/algorithmic-trading) significantly enhances trading efficiency by executing orders at precise times, minimizing latency and the likelihood of human error. Additionally, it facilitates high-frequency trading strategies that leverage small price movements, which can be especially advantageous in the volatile commodities market.

One of the significant applications of algorithmic trading in commodities is the optimization of crush spread execution. Crush spreads, involving soybeans, soybean oil, and soybean meal, require precise timing and execution to maximize profit margins. Algorithms can swiftly process vast amounts of market data, identifying optimal entry and [exit](/wiki/exit-strategy) points for crush spread positions. This capability enables traders to react almost instantaneously to market movements, securing more favorable price spreads.

Several algorithmic strategies are commonly employed in agricultural futures trading. Trend-following algorithms are designed to capitalize on prolonged market movements, adjusting positions in response to sustained price trends. Mean reversion strategies, conversely, exploit short-term price deviations, assuming that prices will revert to an average over time. Additionally, statistical [arbitrage](/wiki/arbitrage) algorithms identify pricing inefficiencies between related instruments, potentially offering risk-free profit opportunities.

Several tools and platforms support algorithmic trading in commodities. For instance, MetaTrader and NinjaTrader provide comprehensive trading environments with robust scripting languages for custom algorithm development. More advanced traders may use Python libraries like Zipline and PyAlgoTrade to build sophisticated trading algorithms. These tools often offer features such as [backtesting](/wiki/backtesting) capabilities, enabling traders to evaluate strategies against historical data before deploying them in live markets.

The integration of algorithmic trading in the commodities sector represents a paradigm shift, providing traders with the tools to manage complex trading strategies with increased speed and precision. As technology advances, the role of algorithms is likely to expand, further enhancing the efficiency and predictability of commodities trading.

## Strategies for Effective Crush Spread Trading

Identifying and leveraging market signals for profitable crush spread trading involves understanding a variety of market dynamics and data indicators. Successful traders analyze factors like price trends in soybeans, soybean oil, and soybean meal, which are the primary components of the crush spread. Key market signals include changes in supply and demand, geopolitical events affecting trade policies, and weather conditions influencing crop yields. Monitoring these signals allows traders to anticipate market movements and execute timely trades, improving profitability.

Risk management strategies specific to crush spread trading are essential to minimize potential losses and optimize returns. Traders often employ hedging techniques to protect against adverse price movements. For instance, a trader might take a long position in soybean oil and meal futures while simultaneously taking a short position in soybean futures to mitigate risks associated with fluctuations in individual commodity prices. Setting stop-loss orders and maintaining a diversified portfolio can also help in managing risks effectively. 

Seasonal patterns play a significant role in predicting price movements in agricultural futures. Historical data often reveal that certain periods, typically corresponding to planting and harvest times, experience predictable volatility. Traders who understand these seasonal trends can position themselves advantageously, opening or closing trades at opportune moments to capitalize on expected price shifts.

Integrating fundamental and technical analysis is crucial for making informed trade decisions. Fundamental analysis involves examining the underlying factors affecting supply and demand, such as crop reports, macroeconomic indicators, and policy changes. Technical analysis, on the other hand, focuses on price data, using charts and technical indicators like moving averages, Relative Strength Index (RSI), and Bollinger Bands to identify patterns and potential entry or exit points. Combining these analytical approaches allows traders to develop a comprehensive strategy, enhancing their ability to predict market movements and execute profitable trades.

Utilizing a Python-based approach, traders can automate the process of analyzing technical signals. Here's a basic example of how one might employ Python to examine moving averages, a common technical indicator:

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

# Assume 'data' is a pandas DataFrame containing historical price data with a 'Date' and 'Close' column
data['SMA_20'] = data['Close'].rolling(window=20).mean()
data['SMA_50'] = data['Close'].rolling(window=50).mean()

plt.figure(figsize=(12, 6))
plt.plot(data['Date'], data['Close'], label='Close Price')
plt.plot(data['Date'], data['SMA_20'], label='20-Day SMA', color='orange')
plt.plot(data['Date'], data['SMA_50'], label='50-Day SMA', color='green')
plt.legend(loc='best')
plt.title('Soybean Futures Moving Averages')
plt.xlabel('Date')
plt.ylabel('Price')
plt.grid(True)
plt.show()
```

This code snippet calculates and plots the 20-day and 50-day simple moving averages (SMA) of soybean futures prices, helping traders identify crossover points that may signal buying or selling opportunities. By integrating such technical analysis into their strategy, traders can make more informed decisions in crush spread trading.

## The Role of Technology and Tools

Technology and tools play a crucial role in trading agricultural futures, enhancing efficiency and precision in a market that is highly sensitive to fluctuations in supply and demand. Efficient trading in this sector requires the integration of advanced technologies, reliable data pathways, and user-friendly platforms that can handle the complexities of futures contracts, such as those for soybeans, corn, and wheat.

### Overview of Technology and Tools

Modern trading of agricultural futures is underpinned by sophisticated technologies and an array of digital tools that cater to different aspects of trading activities. These include algorithmic trading systems, advanced trading platforms, real-time data analytics, and specialized software for risk management. 

### Trading Platforms

Various trading platforms provide users with access to futures markets, each with distinct features tailored to different trading needs. Platforms like the Chicago Mercantile Exchange (CME) Group's Globex, Intercontinental Exchange (ICE), and Euronext offer electronic trading environments with various functionalities. Key considerations for choosing a platform include:

- **Ease of Use**: User-friendliness is crucial for implementing and managing trades efficiently. Platforms with intuitive interfaces and controls help traders execute strategies without unnecessary complications.
- **Market Access**: Comprehensive access to a wide range of futures contracts is essential. Ensuring the platform provides timely updates on agricultural market movements is critical for achieving a competitive edge.
- **Execution Speed**: Fast execution is paramount in futures trading, where market conditions can change rapidly. Low latency platforms can help traders capitalize on minor price movements, crucial for high-frequency trading strategies.
- **Integration Capabilities**: Platforms should integrate seamlessly with third-party tools and proprietary systems, facilitating comprehensive analysis and execution strategies.

### Data Analytics and Real-Time Monitoring

Data analytics is vital for informed decision-making in agricultural futures trading. The sheer [volume](/wiki/volume-trading-strategy) of data generated by global markets necessitates tools capable of processing and analyzing information efficiently.

- **Real-Time Monitoring**: Platforms equipped with real-time data feeds allow traders to monitor market trends as they happen. Access to real-time quotes, news, and financial analysis is critical for responding to market movements instantaneously.
- **Predictive Analytics**: Leveraging predictive models helps traders anticipate market trends based on historical data and market signals. Machine learning algorithms can refine these models continually, improving their accuracy.
- **Risk Management**: Through sophisticated analytics, traders can assess risk factors, model potential market scenarios, and develop strategies to mitigate losses. Tools that offer custom alerts and comprehensive reporting systems enhance a trader's ability to react to and manage risks effectively.

### Selecting Trading Software

Choosing the right trading software is crucial for supporting algorithmic trading strategies. Such software should facilitate seamless execution, offer backtesting capabilities, and integrate with various data sources.

- **Algorithm Development**: Effective software provides environments for creating and testing algorithms using historical data. Python is a widely used language for these tasks, thanks to its libraries such as NumPy, pandas, and scikit-learn, which aid in numerical computations and machine learning.

  ```python
  import numpy as np
  import pandas as pd

  # Sample code snippet for calculating moving averages, a common trading algorithm component
  data = pd.read_csv('futures_data.csv')
  data['Moving_Average'] = data['Price'].rolling(window=20).mean()
  ```

- **Backtesting**: The ability to simulate trading strategies on historical data allows traders to evaluate their effectiveness before deploying them in live markets. This function helps refine strategies to maximize profitability and manage risks.
- **Automation Capabilities**: Automation is a critical feature, allowing for the execution of trades based on pre-set criteria. This reduces emotional decision-making, ensuring trades are executed based on strategic parameters.

The integration of technology and advanced tools is essential for modern agricultural futures trading. By selecting the right platforms and software, employing robust data analytics, and harnessing real-time monitoring, traders can enhance their ability to manage trades efficiently, mitigate risks, and capitalize on market opportunities.

## Case Studies and Real-World Applications

The application of crush spreads and algorithmic trading in agricultural futures has yielded notable success stories, demonstrating the profitability and efficiency of these strategies. One such example involves a commodities trading firm that leveraged algorithmic trading to optimize its crush spread strategies. By employing a sophisticated algorithm that accounted for real-time market data, the firm was able to quickly respond to volatility in soybean, soybean oil, and soybean meal prices. This approach not only enhanced their profit margins but also significantly reduced exposure to market risks. The algorithm worked by continuously recalculating the optimal spread position, thus enabling the firm to dynamically adjust their positions and lock in favorable margins. Such a strategy allowed the firm to outperform manual trading techniques, showcasing the potential of algorithmic trading in commodities markets.

Analysis of historical data has shown that crush spreads can considerably impact trading outcomes. For instance, during a period of heightened volatility in the soybean market due to geopolitical tensions affecting global supply chains, traders who effectively utilized crush spreads were able to hedge against adverse price movements. Historical data analysis indicated that traders employing crush spreads realized gains as they were able to secure more predictable profit margins despite fluctuating primary commodity prices. This success was largely attributed to the crush spread's inherent ability to balance risks associated with the simultaneous purchase of raw soybeans and sale of its derivative products, soybean oil and meal.

Lessons learned from past trading scenarios underline the importance of adaptability and comprehensive market understanding. A key insight is the need to integrate both [fundamental analysis](/wiki/fundamental-analysis)—such as supply and demand forecasts, weather patterns, and geopolitical events—and technical analysis to anticipate price movements effectively. Traders who combined these analyses with algorithmic strategies were better positioned to exploit market opportunities and mitigate potential losses.

Furthermore, successful traders often emphasized the critical role of technology and real-time data analytics in refining their trading strategies. By leveraging advanced data analytics platforms, traders were able to monitor market trends instantaneously and make informed decisions promptly. This technological edge was particularly beneficial during periods of unforeseen market changes, where timely adjustments were paramount to maintaining profitability. 

These case studies and historical analyses underscore the potential benefits of employing crush spreads and algorithmic trading in agricultural futures. They serve as instructive examples for traders seeking to enhance their market strategies and operational efficiency. The key takeaway is that by combining traditional spread strategies with modern technological tools, traders can achieve superior results in managing price risks and optimizing their trading performance.

## Conclusion

Crush spreads hold significant importance in agricultural futures trading, particularly within the soybean market. They serve as a critical risk management tool, allowing traders to hedge against price volatility by offsetting the purchase of raw soybeans with sales of its derivative products—soybean oil and soybean meal. This strategic approach helps stabilize potential uncertainties and smoothens profit margins for those involved in soybean processing and trading.

Algorithmic trading emerges as a powerful ally in enhancing trading efficiency. By leveraging algorithmic strategies, traders can execute complex trades rapidly and accurately, responding swiftly to market changes. Algorithms facilitate the optimization of crush spreads by analyzing vast data sets to identify profitable opportunities, manage risks, and implement trades at the most advantageous moments.

Looking forward, the future of commodities trading in the agricultural sector appears promising, driven by advancements in technology and data analytics. The integration of [machine learning](/wiki/machine-learning) and [artificial intelligence](/wiki/ai-artificial-intelligence) in trading algorithms is likely to transform how traders analyze market signals, predict trends, and make decisions. These technological enhancements promise to further increase the precision and speed of trade executions, ultimately making the market more efficient and accessible.

Traders are encouraged to explore and implement these advanced strategies to remain competitive and capitalize on emerging opportunities in an ever-evolving market landscape. By adopting both crush spread strategies and algorithmic trading, market participants can better navigate price fluctuations and tap into the full potential of agricultural futures trading. This proactive approach not only aids in securing sustained profitability but also contributes to the overall stability and growth of the agricultural commodities market.

## Additional Resources

### Suggested Readings and Guides on Commodities Trading and Spreads

For those seeking to deepen their understanding of commodities trading and spreads, several authoritative texts and resources can provide valuable insights. "Commodity Derivatives: Markets and Applications" by Neil C. Schofield offers a comprehensive overview of various commodity markets, including agricultural futures, and a detailed analysis of trading strategies such as spreads. Additionally, "Option Volatility and Pricing" by Sheldon Natenberg can be particularly useful for understanding the intricacies of pricing strategies, including spread techniques.

### Links to Platforms Offering Algorithmic Trading for Beginners

Algorithmic trading platforms are essential for those looking to refine their trading strategies using technology. For beginners, platforms like QuantConnect (https://www.quantconnect.com/) and Alpaca (https://alpaca.markets/) offer user-friendly interfaces and comprehensive tutorials. These platforms provide access to historical data and allow users to backtest their models, making them ideal for those new to algorithmic trading.

#### QuantConnect Example:

```python
from AlgorithmImports import *

class BasicTemplateAlgorithm(QCAlgorithm):
    def Initialize(self):
        self.SetStartDate(2020, 1, 1)  # Set Start Date
        self.SetCash(100000)  # Set Strategy Cash
        self.AddEquity("SPY", Resolution.Daily)

    def OnData(self, data: Slice):
        if not self.Portfolio.Invested:
            self.SetHoldings("SPY", 1)
```

This Python example initializes a simple algorithm using QuantConnect to trade SPY based on historical data, which can be adapted for more complex agricultural futures strategies.

### Access to Tools and Services for Real-Time Data and Trading Support

Real-time data access and robust trading support services are critical for successful commodities trading. Bloomberg Terminal (https://www.bloomberg.com/professional/solution/bloomberg-terminal/) offers extensive real-time data and analysis tools for professional traders. For those seeking a more accessible option, TradingView (https://www.tradingview.com/) provides community-driven analysis and charting tools suitable for both beginners and experienced traders.

Furthermore, platforms such as [Interactive Brokers](/wiki/interactive-brokers-api) (https://www.interactivebrokers.com/) integrate industry-leading data services and algorithmic trading capabilities, allowing traders to execute sophisticated strategies efficiently. Access to these resources can significantly enhance decision-making and improve trading outcomes in agricultural futures markets.

## References & Further Reading

[1]: Hull, J. C. (2012). ["Options, Futures, and Other Derivatives"](https://www.semanticscholar.org/paper/Options%2C-Futures%2C-and-Other-Derivatives-Hull/89bdee500c8623864fc9eb7a471546aa713acc44) (8th ed.). Pearson Education.

[2]: Achelis, S. B. (2001). ["Technical Analysis from A to Z"](https://archive.org/details/technicalanalysi00ache) (2nd ed.). McGraw Hill.

[3]: Porteous, S. D., & Lord, J. L. (2002). ["Commodity Exchanges and Futures Trading: Principles and Operating Methods."](https://archive.org/details/commodityexchang0000juli)

[4]: Murphy, J. J. (1999). ["Technical Analysis of the Financial Markets: A Comprehensive Guide to Trading Methods and Applications."](https://archive.org/details/technicalanalysi0000murp) New York Institute of Finance.

[5]: Irwin, S. H., & Sanders, D. R. (2012). ["Financialization and Structural Change in Commodity Futures Markets."](https://caia.org/sites/default/files/membersonly/Financialization_and_Structural_Change_in_Commodity_Future_Markets.pdf) Journal of Agricultural and Applied Economics, 44(3).

[6]: Chan, E. P. (2009). ["Quantitative Trading: How to Build Your Own Algorithmic Trading Business"](https://github.com/ftvision/quant_trading_echan_book). John Wiley & Sons.

[7]: Kaminski, V. (2004). "The Economics of Commodity Trading Firms." [Global Commodities: A History and Evolution](https://www.bauer.uh.edu/spirrong/economics-commodity-trading-firms.pdf). Cambridge Resources International.

[8]: Lopez de Prado, M. M. (2018). ["Advances in Financial Machine Learning"](https://www.amazon.com/Advances-Financial-Machine-Learning-Marcos/dp/1119482089). Wiley.