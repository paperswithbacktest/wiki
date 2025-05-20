---
category: trading_strategy
description: 3Red Partners excels in algorithmic trading by leveraging advanced technology
  and a collaborative culture to navigate financial markets with precision and innovation.
title: 3Red Partners (Algo Trading)
---

![Image](images/1.png)

## Table of Contents


**3Red Partners** is a global proprietary trading firm founded in 2011 that leverages technology and quantitative research to implement a diverse set of algorithmic trading strategies while actively managing risk in dynamic markets. Headquartered in Chicago, the firm is known for its use of high-frequency trading (HFT), statistical arbitrage, and market-making strategies across various financial markets. 3Red Partners operates as an **algorithmic trading** company (using computer-driven trading programs) and **proprietary trading firm** (trading its own capital) with a focus on **quantitative trading** techniques.

## History

3Red Partners was co-founded by **Igor Oystacher**, a former trader at Gelber Group, along with **Edwin Johnson** (also from Gelber) in late 2010. Oystacher left Gelber in 2010 to start the new proprietary trading venture, establishing 3Red’s operations in Chicago, Illinois. The firm officially began trading in 2011, initially with a small team of traders and technologists. Over time, 3Red grew into a mid-sized trading shop, reportedly employing on the order of 100+ staff including quantitative researchers, engineers, and traders. The company’s Chicago headquarters is in the city’s financial district, and it has expanded its trading activities to exchanges and markets worldwide.

From its inception, 3Red Partners made headlines for its aggressive trading tactics. The firm trades a wide range of asset classes, including equity index futures, commodities, and other derivatives. For example, 3Red (and Oystacher) have been active in futures contracts ranging from the S\&P 500 E-mini and VIX volatility index to crude oil, natural gas, and copper. In the mid-2010s, 3Red became entangled in regulatory scrutiny when U.S. authorities alleged that Oystacher engaged in “**spoofing**” – a manipulative high-speed trading practice. In 2016, the U.S. Commodity Futures Trading Commission (CFTC) settled a lawsuit with Oystacher and 3Red, with the firm paying a \$2.5 million penalty for allegedly placing and canceling large orders to mislead the market. Despite these legal challenges, 3Red continued to operate after instituting stricter compliance measures. By 2019, **George Monogyios** (formerly of Tower Research) joined 3Red as a Managing Partner and Head of Trading to help expand its quantitative trading business. As of 2025, Oystacher remains CEO, and 3Red Partners is regarded as one of the notable Chicago-based high-frequency trading firms, alongside competitors like Jump Trading and DRW, known for its sophisticated strategies and cutting-edge trading infrastructure.

## Trading Strategies

3Red Partners employs a variety of **algorithmic trading strategies** to profit from inefficiencies in financial markets. Its approach is rooted in quantitative models and **automation**, allowing the firm’s algorithms to trade large volumes at extremely high speed. The primary strategies 3Red is associated with include **high-frequency trading (HFT)**, **statistical arbitrage (stat arb)**, and **market-making**. Each of these quantitative trading strategies plays a role in the firm’s overall trading portfolio:

### High-Frequency Trading (HFT)

**High-frequency trading** is a cornerstone of 3Red’s operations. HFT is a subset of algorithmic trading characterized by extremely high-speed trade execution, high turnover rates, and very short holding periods. HFT firms like 3Red rely on highly sophisticated algorithms and co-located trading servers to execute orders in fractions of a second. The goal of HFT strategies is often to capture tiny price discrepancies or momentum effects at the microsecond to millisecond level, accumulating profit through a large number of rapid trades. Key attributes of HFT include the use of direct market access and ultra-low latency connections to exchanges, as well as very short-term investment horizons (positions may be held only for seconds or less). 3Red’s algorithms continuously scan multiple markets and order books for opportunities, making split-second decisions that are impossible for manual traders. By leveraging speed, HFT strategies aim to exploit minute price differences or liquidity imbalances before other market participants can react. The firm’s trading programs are designed to handle high order volumes and update orders at rates that approach hardware and network limits. This focus on maximum speed and minimal latency gives 3Red a competitive edge in **algorithmic trading** competition, where success is often measured in microseconds.

### Statistical Arbitrage

Another core strategy at 3Red Partners is **statistical [arbitrage](/wiki/arbitrage)**, a [quantitative trading](/wiki/quantitative-trading) technique that seeks to profit from statistical patterns in asset prices. Statistical arbitrage (often abbreviated as *stat arb*) strategies use **mean reversion** analysis and correlation patterns to identify mispricings among securities. Traders construct a portfolio of assets—often taking both long and short positions—to exploit temporary deviations from historical price relationships. These strategies are typically **market-neutral**, meaning the portfolio is structured to cancel out broad market risk by pairing long and short positions in related instruments. For example, a stat arb algorithm might detect that **Coca-Cola** and **PepsiCo** shares, which usually move in tandem, have diverged in price. The strategy could go long the undervalued stock (Coke) and short the overvalued stock (Pepsi), betting that their price spread will revert to the mean. Such pairs trading is a classic form of stat arb.

Statistical arbitrage at high frequencies involves large-scale data analysis and often a multitude of instruments. The algorithms identify predictable, short-lived **pricing anomalies** or **spread divergences** among baskets of correlated assets. These opportunities might arise from temporary supply-demand imbalances or lags in how information is reflected across related markets. 3Red’s systems continuously “score” securities based on quantitative factors and seek to exploit those small inefficiencies before they vanish.  Because stat arb assumes prices will revert to a statistical norm, **mean reversion models** are a fundamental tool. A common mathematical model for a mean-reverting process is the Ornstein–Uhlenbeck formulation:

$$
dX_t = \theta (\mu - X_t)\,dt + \sigma\,dW_t\,,
$$

where \$X\_t\$ is the price (or spread) at time \$t\$, \$\mu\$ is its long-term mean value, \$\theta\$ is the speed at which \$X\_t\$ reverts toward \$\mu\$, \$\sigma\$ is the volatility, and \$dW\_t\$ is a random fluctuation term. This stochastic differential equation is often used to model how a price *pulls back* toward an equilibrium level over time. In practice, 3Red’s analysts calibrate such models to historical data to forecast the likelihood and speed of mean reversion in various trading signals. Stat arb trades are typically held for short durations (sometimes only seconds or minutes in HFT contexts, or a few days for slower mean reversion plays). The firm’s quantitative strategies manage a large number of small positions, expecting that on average the small profits per trade will accumulate due to the high frequency of occurrences.

### Market-Making

**Market-making** is another important aspect of 3Red Partners’ trading operations. In a market-making strategy, the trading firm continuously provides **liquidity** to the market by posting both buy and sell orders (bids and asks) for various financial instruments. 3Red’s algorithms act as automated market makers, offering to buy at slightly below the current market price and sell at slightly above it, thereby capturing the **bid-ask spread** as profit. By constantly quoting prices and updating them in real-time, the firm ensures there is always a market for the securities it trades, earning small gains on the spread with each transaction.

Market makers like 3Red play a crucial role in electronic markets by enhancing [liquidity](/wiki/liquidity-risk-premium) and reducing transaction costs. The firm’s trading systems are designed to handle a high [volume](/wiki/volume-trading-strategy) of order updates, adjusting quotes in response to market movements or new information in milliseconds. **Risk management** is integral to market-making: the algorithms must dynamically manage inventory (the net position in each asset) and avoid accumulating too large a position in one direction. 3Red’s market-making programs use quantitative models to price assets and determine fair value, and they use **fast-feedback loops** to cancel or update quotes to avoid being adversely selected by faster traders. According to industry reports, many [HFT](/wiki/high-frequency-trading-strategies) firms earn significant income from liquidity rebates and market-making operations — for example, some exchanges offer fee rebates to participants who supply liquidity. 3Red’s presence in the order [books](/wiki/algo-trading-books) helps tighten bid-ask spreads, and in return the firm aims to earn consistent, if small, profits on a large number of trades. This strategy leverages both the firm’s speed advantage and its ability to manage many small positions simultaneously. While market-making has relatively low profit per trade, the [high frequency](/wiki/high-frequency-trading) and volume of trades can generate substantial cumulative profits, and the strategy tends to perform well in markets with sufficient [volatility](/wiki/volatility-trading-strategies) and volume.

## Technology and Infrastructure

Operating as a high-performance [algorithmic trading](/wiki/algorithmic-trading) firm, 3Red Partners relies on cutting-edge technological infrastructure and rigorous quantitative analysis. **Technical infrastructure** is a critical [factor](/wiki/factor-investing) in 3Red’s success, as the speed and reliability of its trading systems directly impact profitability. The firm employs a combination of advanced hardware, software, and network solutions to achieve ultra-low latency (minimal delay) in both trade execution and data processing.

On the hardware and network side, 3Red uses co-located servers placed directly in or near exchange data centers, which drastically reduces the time it takes for orders to reach the exchange matching engines. By being physically close to the exchanges (in Chicago, New York, London, etc.), the firm’s trading engines can execute and cancel orders faster than competitors farther away. Moreover, 3Red has invested in specialized network connectivity between major financial hubs. For instance, many HFT firms have moved from traditional fiber-optic communication lines to microwave or other wireless technologies for long-distance data transmission, since signals through the air travel faster than through fiber cables. A microwave link between Chicago and New York can transmit market data with a few milliseconds advantage over fiber networks. 3Red leverages such low-latency networks to gain timing advantages in cross-market strategies (for example, arbitraging price differences between CME in Chicago and exchanges in New York). The firm’s trading hardware includes custom-built **high-speed processors** and can even involve **FPGA** (Field-Programmable Gate Array) hardware accelerators for nanosecond-level optimizations, as is increasingly common in HFT infrastructure. These technologies enable 3Red’s systems to handle massive streams of market data and make split-second decisions with minimal delay.

On the software side, 3Red Partners combines **high-performance code** for execution with flexible research platforms for strategy development. Critical real-time components (such as order routing, risk checks, and strategy execution) are often written in low-level, highly optimized programming languages like C++ to maximize speed. Meanwhile, the firm’s quantitative researchers use languages and tools like Python, R, or MATLAB for data analysis, simulation, and model development. This two-tiered approach allows 3Red to maintain an efficient production trading system while fostering rapid research and innovation. The company maintains a vast repository of historical market data for [backtesting](/wiki/backtesting) strategies under realistic conditions. Researchers at 3Red utilize distributed computing and **high-performance computing clusters** to run computationally intensive backtests and optimizations. For example, testing a new [statistical arbitrage](/wiki/statistical-arbitrage) model may involve simulating it on years of tick-by-tick data across dozens of instruments, requiring significant computational power.

Another crucial element of 3Red’s infrastructure is **risk management and analytics**. In a fast-paced proprietary trading environment, risk controls must be automated and operate in real-time. 3Red’s trading platform incorporates real-time risk checks that monitor positions, exposure, and market conditions, with the ability to automatically halt trading if certain thresholds are breached. The firm uses mathematical models to quantify risk measures such as **volatility** and potential losses. Volatility – a measure of how much an asset’s price fluctuates – is particularly important for calibrating strategy parameters and setting risk limits. It is often calculated as the standard deviation of returns. For example, if \$r\_1, r\_2, \dots, r\_N\$ are daily returns of an asset, the annualized volatility \$\sigma\$ might be computed as:

$$
\sigma \;=\; \sqrt{252 \;\frac{1}{N}\sum_{t=1}^{N}(r_t - \bar{r})^2}\,,
$$

where \$\bar{r}\$ is the average daily return and 252 is the number of trading days in a year. This formula gives the trader an estimate of the asset’s variability (on an annualized basis) by scaling the daily return variance. 3Red’s systems constantly update such risk metrics for each strategy and trading portfolio. The firm also employs **analytics dashboards** for its traders and risk managers, providing real-time feedback on profit & loss, position sizes, and performance attribution of various strategies. By combining robust risk management with their technical infrastructure, 3Red aims to prevent catastrophic losses and ensure that no single strategy or erroneous algorithm trade can jeopardize the firm. This blend of technology and quantitative rigor in 3Red’s infrastructure has been a key factor in its ability to compete in the highly demanding domain of high-frequency and quantitative trading.

## Strategy Simulation Example

To illustrate the type of quantitative strategies a firm like 3Red Partners might deploy, consider a simplified **mean reversion trading strategy** implemented in Python. We will use the **Backtrader** framework (a popular open-source library for backtesting trading strategies) and historical price data from the *Papers With Backtest* toolbox (pwb-toolbox). The strategy in this example monitors a single stock’s price relative to its moving average and executes trades based on deviations – a basic proxy for statistical arbitrage on a single asset. When the price falls sufficiently below the moving average (indicating a potential undervaluation), the strategy will buy, expecting a reversion upward; conversely, if the price rises well above the average (potential overvaluation), the strategy will sell or go short. This simple logic emulates the mean-reverting principle in stat arb, albeit on one instrument for clarity.

Below is an example code snippet that sets up the backtesting environment using Backtrader and the pwb-toolbox data. The code defines a custom strategy, retrieves historical pricing data for a stock (e.g., Apple Inc.), and runs a backtest of the strategy:

```python
import backtrader as bt
import pwb_toolbox.datasets as pwb_ds
import pandas as pd

# Define a simple mean-reversion strategy for Backtrader
class MeanReversionStrategy(bt.Strategy):
    params = (('lookback', 20), ('threshold', 0.05),)
    
    def __init__(self):
        # Compute a simple moving average over the lookback window
        self.sma = bt.indicators.SimpleMovingAverage(self.data.close, period=self.p.lookback)
    
    def next(self):
        # Calculate the divergence of price from the moving average
        price = self.data.close[0]
        avg   = self.sma[0]
        if price < avg * (1 - self.p.threshold):
            # Price is significantly below average -> mean reversion buy signal
            if not self.position:      # only buy if not already in position
                self.buy()
        elif price > avg * (1 + self.p.threshold):
            # Price is significantly above average -> mean reversion sell signal
            if self.position:          # sell if we have a position
                self.sell()

# Load historical daily price data for a stock (e.g., AAPL) from the PWB toolbox
df = pwb_ds.get_pricing(["AAPL"])        # DataFrame with AAPL price history
df = df["AAPL"] if "AAPL" in df else df  # select AAPL column if dataset returns multi-column DataFrame
df = df.dropna()                         # drop any missing values
# Ensure the DataFrame index is datetime and sorted (required by Backtrader)
df.index = pd.to_datetime(df.index)
df.sort_index(inplace=True)

# Set up Backtrader engine and feed the data
data_feed = bt.feeds.PandasData(dataname=df, open='Open', high='High', low='Low', close='Close', volume='Volume')
cerebro = bt.Cerebro()
cerebro.addstrategy(MeanReversionStrategy)
cerebro.adddata(data_feed)
cerebro.run()

# Plot or analyze the results (e.g., final portfolio value, trade log) as needed
```

In this code, we first import the necessary libraries: **Backtrader** for the backtesting engine and `pwb_toolbox.datasets` for retrieving market data. We define `MeanReversionStrategy` as a subclass of `bt.Strategy` with two parameters: a `lookback` period for the moving average (20 days) and a `threshold` (5% deviation). In the strategy’s `next()` method (called on each new time step), the current closing price is compared to the moving average. If the price dips more than 5% below the average, the strategy issues a buy order (entering a long position) assuming the price will revert upward. If the price rises more than 5% above the average and a position is held, the strategy sells (exits the position) to capture profits from the mean reversion.

We then load historical data for Apple (“AAPL”) using the PWB toolbox. The data is loaded into a pandas DataFrame `df` with columns for Open, High, Low, Close, etc. After some minor formatting (ensuring the index is a datetime index and sorted in chronological order), we create a Backtrader `PandasData` feed from the DataFrame. Next, we set up a `Cerebro` engine (Backtrader’s backtesting engine), add our `MeanReversionStrategy`, and add the data feed to it. Finally, we run the backtest with `cerebro.run()`.

When executed, this backtest would simulate the strategy on Apple’s historical prices. One could then examine the performance of the strategy – for instance, looking at the profit and loss, the number of trades executed, and how closely the strategy managed to buy at low deviations and sell at high deviations. In a more elaborate setup, 3Red’s traders would extend this concept to multiple securities and include more complex statistical measures, risk management overlays, and execution logic to handle real market conditions (such as transaction costs and slippage). Nonetheless, this example demonstrates the basic workflow of developing and testing an **algorithmic trading strategy** in a quantitative trading firm: define a hypothesis or model (here, mean reversion), implement the algorithm, backtest it on historical data, and analyze the results for profitability and risk.


## References & Further Reading

[1]: [3Red Partners Overview | SignalHire Company Profile](https://www.signalhire.com/companies/3red-trading)

[2]: [Oystacher Gets a Second Spoofing Fine, This Time From ICE](https://www.tradersmagazine.com/departments/people/oystacher-gets-a-second-spoofing-fine-this-time-from-ice/)

[3]: [Before U.S. Called Oystacher a Spoofer, He Was Known as 990](https://www.tradersmagazine.com/departments/buyside/before-u-s-called-oystacher-a-spoofer-he-was-known-as-990/)

[4]: [Federal Court Orders Chicago Trader Igor B. Oystacher and 3Red Trading LLC to Pay \$2.5 Million Penalty | CFTC](https://www.cftc.gov/PressRoom/PressReleases/7504-16)

[5]: [Prop trading firm adds new managing partner as hiring ramps up | eFinancialCareers](https://www.efinancialcareers.com/news/2019/02/prop-trading-firm-hiring-3red)

[6]: [3Red Partners - Leadership Team | The Org](https://theorg.com/org/3red-partners/teams/leadership-team)

[7]: [High-frequency trading - Wikipedia](https://en.wikipedia.org/wiki/High-frequency_trading)

[8]: [Strategies And Secrets of High Frequency Trading (HFT) Firms | Investopedia](https://www.investopedia.com/articles/active-trading/092114/strategies-and-secrets-high-frequency-trading-hft-firms.asp)

[9]: [Statistical Arbitrage: Definition, How It Works, and Example | Investopedia](https://www.investopedia.com/terms/s/statisticalarbitrage.asp)

[10]: [GitHub - paperswithbacktest/pwb-toolbox](https://github.com/paperswithbacktest/pwb-toolbox)