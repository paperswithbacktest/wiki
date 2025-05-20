---
category: trading_strategy
description: Discover the importance of backtesting in algo trading – a methodical
  process that simulates trading strategies using historical data. Learn how it helps
  assess strategy feasibility, refine approaches, and provides valuable insights for
  improved performance.
title: Backtesting for Algo Trading
---

Backtesting, in trading and finance, is a methodical process where traders simulate their trading strategies using historical data. This simulation allows traders to see how their strategy would have performed in the past, making it a vital tool for assessing the feasibility of a trading plan before risking actual capital. The primary aim is to validate the strategy's effectiveness and to refine it if necessary.

![Untitled](images/Untitled.png)

The significance of backtesting cannot be overstated. It offers traders a glimpse into the potential future performance of their strategies. Without backtesting, traders would have to rely solely on real-time trades to evaluate their strategies, which could be costly and time-consuming. By simulating trades using past data, traders can identify potential flaws or strengths in their strategy, allowing for optimization before live trading. Furthermore, backtesting provides an empirical foundation, adding a layer of confidence in the trading approach. It's akin to a rehearsal before the main performance, ensuring that traders are better prepared for the dynamic world of financial markets.

However, it's worth noting that while backtesting is a powerful tool, it is not without its limitations. A strategy's past performance, as reflected in backtest results, does not guarantee future results. Market conditions change, and unexpected events can influence outcomes. Nonetheless, when used correctly and with an understanding of its intricacies, backtesting remains an indispensable component in a trader's toolkit.

## Table of Contents

## Foundations of Backtesting

Backtesting is the process of testing a trading strategy using historical market data to evaluate its viability. In essence, it involves simulating trades that would have been executed in the past using the rules defined by the strategy. By observing the hypothetical results of these trades, traders can gain insight into the potential profitability and risk of their strategy without committing actual capital.

The core concepts underlying backtesting revolve around data integrity, realism, and objectivity. Accurate historical data is paramount; without it, the backtest results could be misleading. Realism pertains to the importance of incorporating realistic trading conditions, such as slippage, transaction costs, and liquidity constraints, to obtain results that are as close as possible to real-world outcomes. Objectivity ensures that the testing process remains unbiased, avoiding common pitfalls such as data snooping and overfitting.

Historically, [backtesting](/wiki/backtesting) as a concept has deep roots, but its modern form evolved with the rise of computers and digitized data. In the early days of trading, chartists would manually plot market prices on paper to identify patterns and trends. These rudimentary methods had their limitations due to the tedious nature of manual calculations and the potential for human error. However, as technology advanced, especially in the late 20th century, traders gained access to sophisticated software that could process vast amounts of data rapidly. This technological leap marked the transformation of backtesting from a largely manual, time-consuming process to an automated, efficient one[1].

The evolution of backtesting is intrinsically linked to the broader shifts in the trading world. The proliferation of [algorithmic trading](/wiki/algorithmic-trading), where computers are programmed to execute trades based on a set of predefined criteria, further underscored the importance of backtesting. As markets became more competitive and margins thinner, the need for robust, evidence-based strategies became paramount. Backtesting, with its ability to provide empirical evidence on a strategy's merits, naturally found its place at the heart of this new trading paradigm.

In essence, backtesting has grown from manual chart plotting to an indispensable tool in the modern trader's arsenal, helping navigate the complexities of today's financial markets with greater confidence and precision.

## The Mechanics of Backtesting

### How Does Backtesting Work?

At its core, backtesting is a systematic process that allows traders to recreate historical market conditions to test their trading strategies. The aim is to determine how a particular strategy would have performed in the past, which can provide valuable insights into its potential future performance. Here's a breakdown of the steps involved:

1. **Gathering Relevant Data**: The foundation of any backtest is high-quality historical data. This includes price data (open, high, low, close), volume data, and any other relevant market indicators. It's essential to ensure that the data is accurate and free from gaps or errors. The granularity of the data (daily, hourly, minute-by-minute) will depend on the trading strategy being tested. For instance, a long-term investment strategy might rely on daily or weekly data, while a high-frequency trading strategy would require tick-by-tick data.
2. **Formulating a Trading Hypothesis**: Before running a backtest, traders need to have a clear trading hypothesis in place. This hypothesis outlines the specific conditions under which trades will be entered and exited. It might be based on technical indicators, fundamental analysis, or a combination of both. For example, a simple moving average crossover strategy might buy an asset when its short-term moving average crosses above its long-term moving average and sell when the opposite occurs.
3. **Simulation and Results**: With the data and hypothesis in hand, the actual backtest can be conducted. Using specialized backtesting software, the trading strategy is applied to the historical data, simulating trades as if they were made in real-time based on the strategy's rules. The simulation will produce a series of results, including the number of trades made, the percentage of winning trades, total profit or loss, drawdowns, and other critical metrics. These results offer a snapshot of how the strategy would have performed during the period tested.

It's worth noting that while backtesting provides valuable insights, it's not a guarantee of future performance. Markets evolve, and past conditions may not necessarily replicate in the future. However, by rigorously testing a strategy against historical data, traders can gain a better understanding of its strengths, weaknesses, and potential areas for improvement.

### Implementing Backtesting

Implementing backtesting involves a series of meticulous steps, each contributing to the validity and accuracy of the results. When undertaken with attention to detail and the right tools, backtesting can serve as an indispensable tool in a trader's arsenal.

**Steps to Conduct a Thorough Backtest**:

1. **Data Collection**: Begin by acquiring quality historical data. This data should be high resolution, free of gaps, and representative of the market conditions you want to test. Ensure it spans a significant time period to account for different market conditions.
2. **Data Cleaning**: Process the data to remove any errors, outliers, or missing values. Consistent and clean data is fundamental for accurate backtesting.
3. **Determine Testing Parameters**: Before running the backtest, decide on parameters like initial capital, lot size, leverage, and other specific conditions that match your intended trading setup.
4. **Formulate Your Trading Strategy**: Clearly define your strategy's entry and exit rules. This might involve technical indicators, fundamental factors, or a mix of both.
5. **Coding**: Translate your strategy into a computer program. Popular languages for this purpose include Python, R, and C++, among others. This code will take in your historical data and apply your strategy's rules.
6. **Run the Backtest**: With everything set up, execute the backtest. Your code will simulate trades based on your strategy, generating a series of hypothetical trades.
7. **Analyze Results**: Once the backtest concludes, scrutinize the results. Examine key metrics such as return on investment (ROI), maximum drawdown, win/loss ratio, and others to gauge the strategy's performance.

The tools you use play a pivotal role in backtesting. Not only do they affect the accuracy of your results, but they can also impact the efficiency of the process. Superior software will provide a wide range of data analytics tools, visualization options, and will integrate well with your data sources. Furthermore, they should allow for rigorous stress testing and provide insights into various risk [factor](/wiki/factor-investing)s associated with the strategy.

## Data for Backtesting

Financial data comes in different types, including fundamental data, market data, analytics, and [alternative data](/wiki/best-alternative-data).

- Fundamental data is accounting data reported quarterly and contains information that can be found in regulatory filings and business analytics. It is important to confirm the exact time each data point was released to use the information correctly.
- Market data includes all trading activities on an exchange or trading venue, providing an abundant dataset for strategy research.
- Analytics are derivative data based on an original source, processed in a specific way to extract signal for you.
- Alternative data is primary information that has not made it to other sources, which can be expensive and raise privacy concerns, but offers the opportunity to work with unique and hard-to-process datasets.

### Bars

**Time bars**

Periodic “bar” data is the easiest to get. Is sampled at regular intervals (minutely, hourly, daily, weekly) and looks like this:

```
Date,Open,High,Low,Close,Volume
11-May-09,33.78,34.72,33.68,34.35,142775884
12-May-09,34.42,34.48,33.52,33.93,147842117
13-May-09,33.63,33.65,32.96,33.02,175548207
14-May-09,33.10,33.70,33.08,33.39,140021617
15-May-09,33.36,33.82,33.23,33.37,121326308
18-May-09,33.59,34.28,33.39,34.24,114333401
19-May-09,34.14,34.74,33.95,34.40,129086394
20-May-09,34.54,35.04,34.18,34.28,131873676
21-May-09,34.02,34.26,33.31,33.65,139253125

```

“Quote” data shows the best bid and offer:

```
SYMBOL,DATE,TIME,BID,OFR,BIDSIZ,OFRSIZ
QQQQ,20080509,9:36:26,47.94,47.95,931,964
QQQQ,20080509,9:36:26,47.94,47.95,931,949
QQQQ,20080509,9:36:26,47.94,47.95,485,616
QQQQ,20080509,9:36:26,47.94,47.95,485,566
QQQQ,20080509,9:36:26,47.94,47.95,485,576
QQQQ,20080509,9:36:26,47.94,47.95,931,944
QQQQ,20080509,9:36:26,47.94,47.95,849,944
QQQQ,20080509,9:36:26,47.94,47.95,837,944
QQQQ,20080509,9:36:26,47.94,47.95,837,956

```

**Tick bars**

“Tick” or “trade” data shows the most recent trades:

```
SYMBOL,DATE,TIME,PRICE,SIZE
QQQQ,20080509,8:01:29,47.97,1000
QQQQ,20080509,8:01:56,47.97,500
QQQQ,20080509,8:01:56,47.97,237
QQQQ,20080509,8:02:20,47.98,160
QQQQ,20080509,8:02:50,47.98,100
QQQQ,20080509,8:02:50,47.98,200
QQQQ,20080509,8:02:50,47.98,1700
QQQQ,20080509,8:02:50,47.98,500
QQQQ,20080509,8:02:53,47.98,100

```

“Order book” data shows every order submitted and canceled. If you do not know what it looks like, then odds are you do not have the resources to be fast enough to trade on it, so do not worry about it.

**Volume bars**

Volume bars circumvent that problem by sampling every time a pre-defined amount of the security’s units (shares, futures contracts, etc.) have been exchanged. For example, we could sample prices every time a futures contract exchanges 1,000 units, regardless of the number of ticks involved.

Tick bars can introduce arbitrariness in the number of ticks and order fragmentation, while [volume](/wiki/volume-trading-strategy) bars sample every time a pre-defined amount of the security's units have been exchanged, resulting in better statistical properties and providing a convenient artifact for analyzing the interaction between prices and volume in market microstructure theories.

**Dollar bars**

Dollar bars are formed by sampling an observation every time a pre-defined market value is exchanged, which is more reasonable than sampling by tick or volume when the analysis involves significant price fluctuations. The number of outstanding shares often changes multiple times over the [course](/wiki/best-algorithmic-trading-courses) of a security’s life, as a result of corporate actions, and dollar bars tend to be robust in the face of those actions. Thus, dollar bars are more interesting than time, tick, or volume bars.

**Tick Imbalance Bars**

The tick rule defines a sequence of tick imbalances in a given sequence of ticks, where the imbalance is defined as the accumulation of signed ticks exceeding a given threshold. Tick imbalance bars (TIBs) are then defined as T-contiguous subsets of ticks that meet a certain condition. TIBs are more likely to occur when there is informed trading and can be thought of as containing equal amounts of information.

**Volume/Dollar Imbalance Bars**

The concept of tick imbalance bars (TIBs) is extended to volume imbalance bars (VIBs) and dollar imbalance bars (DIBs) to sample bars when volume or dollar imbalances diverge from expectations. The procedure to determine the index of the next sample involves computing the expected value of the imbalance at the beginning of the bar and defining VIB or DIB as a T-contiguous subset of ticks such that the expected imbalance exceeds a given threshold. The bar size is adjusted dynamically, making it more robust to corporate actions.

**Tick Runs Bars**

TIBs, VIBs, and DIBs are methods to monitor order flow imbalance in terms of ticks, volumes, and dollar values exchanged. Tick runs bars (TRBs) measure the sequence of buys in the overall volume and take samples when that sequence diverges from our expectations. TRBs count the number of ticks of each side without offsetting them and are useful in forming bars. The expected value of the current run can be estimated using exponentially weighted moving averages.

**Volume/Dollar Runs Bars**

Volume runs bars (VRBs) and dollar runs bars (DRBs) are based on the same concept as tick runs bars (TRBs), but they monitor volume or dollar imbalances instead of tick imbalances. The procedure to determine the index T of the last observation in the bar is similar to TRBs, and it involves defining the volumes or dollars associated with a run, and defining a VRB or DRB as a T-contiguous subset of ticks such that the expected volume or dollar from runs exceeds our expectation for a bar.

### Sampling

Applying an ML algorithm on an unstructured financial dataset is generally not a good idea due to scalability issues and lack of relevant examples. Sampling bars after certain catalytic conditions can help to achieve a more accurate prediction.

**Sampling for Reduction**

Downsampling is a way to reduce the amount of data used to fit the ML algorithm by sequentially sampling at a constant step size (linspace sampling) or by random uniform sampling. Linspace sampling has the advantage of being simple, but it suffers from arbitrary step size and outcomes that depend on the seed bar. Uniform sampling is better as it draws samples uniformly from the entire set of bars, but it may still not include the most relevant observations in terms of predictive power or informational content.

**Event-Based Sampling**

Portfolio managers make investment decisions after significant events occur, such as changes in market conditions or economic indicators. These events are used to train machine learning algorithms to predict future outcomes. If the algorithm is not accurate, the definition of a significant event may need to be adjusted or alternative features considered.

In financial time series, the signal-to-noise ratio is usually low. Using the entire dataset can cause the model to focus too much on noisy samples and not enough on informative ones. Downsampling can improve the signal-to-noise ratio, but randomly doing so is not effective as it doesn't change the ratio of noisy to informative samples. A better solution is to apply a CUSUM filter, which only creates a sample when the next values deviate sufficiently from the previous value.

Consider a locally stationary process generating IID observations $\{y_t\}_{t=1,..,T}$. The cumulative sums can then be defined as

$$
S_t = \mathrm{max}(0, S_{t-1} + y_t - E_{t-1}[y_t])
$$

with boundary condition $S_{0} = 0$. A sample is only created when $S_{t} \ge h$, for some threshold $h$. This can be further extended to a symmetric CUSUM filter to include run-ups and run-downs such that

$$
S_t^+ = \mathrm{max}(0, S_{t-1}^+ + y_t - E_{t-1}[y_t]), S_o^+ = 0
\\
S_t^- = \mathrm{min}(0, S_{t-1}^- + y_t - E_{t-1}[y_t]), S_o^- = 0
\\
S_t = \mathrm{max}(S_t^+, -S_t^-)
$$

## Aims and Significance of Backtesting

Backtesting stands as a cornerstone in the trading domain for numerous reasons, reinforcing its pivotal role in shaping trading strategies and fostering sound decision-making.

**Strategy Validation**: Before deploying a strategy in live markets, it's imperative to gauge its potential effectiveness. Backtesting allows traders to test their strategies against historical data, providing a hypothetical glimpse into how they would have performed in past market conditions. This offers a chance to tweak and refine strategies before any real money is at risk.

**Risk Management Insights**: One of the most overlooked benefits of backtesting is its capability to provide a clearer view of potential risks. By analyzing metrics like maximum drawdown, volatility of returns, or even the consistency of performance, traders gain insights into the potential downside of their strategies. This can lead to the development of better risk mitigation techniques, such as setting stop-loss orders at optimal points or diversifying trading instruments.

**Enhanced Decision-Making**: Backtesting aids in removing emotions from the trading process. When a strategy is backtested rigorously and shows promising results, traders can confidently follow it, knowing that it has been vetted against vast amounts of data. This leads to more disciplined and systematic trading, reducing the likelihood of impulsive or fear-driven decisions.

**Navigating Financial Markets Confidently**: Financial markets are vast, complex, and constantly evolving. For newcomers and seasoned traders alike, navigating this intricate landscape can be daunting. Backtesting serves as a compass, providing a framework for understanding potential market reactions to various strategies. With a well-tested strategy in hand, traders can approach markets with greater confidence and clarity.

In sum, backtesting is not just a mechanical exercise; it's a crucial process that molds the very foundation of trading. By validating strategies, offering insights into risk, enhancing decision-making, and bolstering confidence, backtesting ensures that traders are equipped to face the dynamic world of financial markets.

## Best Practices & Techniques

### Prerequisites for Effective Backtesting

To achieve meaningful backtest results, one must meticulously set up the right foundational elements. A half-baked or hasty approach can lead to misleading outcomes or strategies that don't truly align with the market's reality.

**Selection Criteria**:

- **Markets**: Choose the market you intend to operate in. While equities are popular, backtesting can be applied across forex, commodities, cryptocurrencies, and more. The choice of market determines data types and granularity needed.
- **Assets**: Narrowing down to specific assets or asset classes is pivotal. A strategy tailored for tech stocks might falter in commodities. Ensure that the asset is aligned with the intended trading strategy and risk appetite.
- **Data**: Quality data is the backbone of backtesting. Prioritize clean, comprehensive, and accurate data sets. They should encompass varying market conditions to stress-test the strategy against different scenarios. Consider factors such as granularity (tick, minute, daily data) and depth (order book data). Websites like Quandl or Yahoo Finance can be useful data sources.
- **Programming Languages**: While many platforms come with built-in backtesting tools, custom backtesting algorithms often offer more flexibility. Python, with libraries like Pandas and Backtrader, is increasingly becoming the go-to choice for many traders. R and MATLAB are also popular for more statistically oriented strategies.

**Timeframes**:
The period for backtesting should align with the strategy's intended holding duration. Day trading strategies might be best tested over shorter periods with high granularity data, while long-term investment strategies might require years of data for accurate evaluation. Also, ensure to include various market conditions, such as bullish, bearish, and sideways markets, to ensure the strategy's robustness across different scenarios.

**Strategy Types**:
A one-size-fits-all approach rarely works in trading. Diversifying strategies is key. Consider trend-following, mean-reversion, [breakout](/wiki/breakout-trading), or [momentum](/wiki/momentum) strategies based on asset behavior and market conditions. For instance, trend-following might excel in commodities, while mean-reversion could be suitable for stable, dividend-paying equities. Research and backtest across diverse strategies to find the most reliable ones for the selected assets and market conditions.

Achieving reliable backtesting results isn't just about running numbers; it's about curating the right environment for those numbers to provide meaningful insights. By carefully choosing markets, assets, and data, determining the right timeframe, and diversifying strategies, traders can lay a robust foundation for backtesting that truly informs and improves their trading endeavors.

### Backtesting with Modern Tools

In today's digital age, traders have access to a myriad of tools designed to simplify and enhance the backtesting process. Leveraging these tools can significantly improve the accuracy and efficiency of strategy evaluation, ensuring that trading approaches are grounded in reality.

**Python**: A leading programming language in the finance sector, Python boasts extensive libraries tailored for backtesting, like [Backtrader](https://www.backtrader.com/), [QuantConnect](https://www.quantconnect.com/), and [PyAlgoTrade](https://gbeced.github.io/pyalgotrade/). These libraries enable users to structure their strategies, feed in historical data, and output performance statistics. With Python, traders can also integrate machine learning techniques to refine their trading algorithms, making it a versatile choice for those seeking deeper analytics.

**MetaTrader 4 (MT4)**: As one of the most popular trading platforms globally, MT4 provides a built-in scripting language, MQL4, for strategy development and backtesting. With its robust charting capabilities and access to historical data directly from brokers, MT4 allows traders to visualize strategy performances over time, all within a familiar trading environment. Its user-friendly interface and community-driven support make it an excellent choice for traders at all levels.

**ProRealTime**: Specializing in technical analysis, ProRealTime offers an intuitive platform with powerful backtesting capabilities. Its advantage lies in the drag-and-drop interface where traders can create strategies without needing to code. The software also emphasizes visualization, enabling users to see strategies play out on historical charts. Additionally, ProRealTime seamlessly integrates with broker accounts, allowing for streamlined transitions from backtesting to live trading.

Visualization is paramount in backtesting. Being able to graphically represent how a strategy would have performed allows traders to identify key moments of opportunity or risk. This visual feedback can be pivotal when fine-tuning or deciding between multiple strategies.

Moreover, a user-friendly interface ensures that the backtesting process is smooth and comprehensible, even for those less technologically inclined. A platform that facilitates easy strategy input, testing modifications, and performance visualization can save traders both time and frustration.

Lastly, community and professional support cannot be understated. Whether it's troubleshooting a coding issue in Python or seeking advice on strategy optimization in MT4, having access to a knowledgeable and active community can be invaluable. Platforms with dedicated forums, tutorials, and customer support provide traders with resources to navigate challenges and continually improve their backtesting endeavors.

When choosing a backtesting tool, it's essential to consider not only its core functionalities but also the broader ecosystem it offers. From visualization to user experience to community support, the right tool can elevate the quality of backtesting and, by extension, the potential success of the trading strategy.

## Evaluating and Interpreting Backtest Results

Assessing the performance of your trading strategy is important, and backtesting the model on a past period is a common way to do this. Metrics such as the Sharpe ratio and maximum drawdown are often used to evaluate financial [machine learning](/wiki/machine-learning) models.

However, a common mistake in backtesting is repeating the backtest multiple times on the same period until a desired result is achieved. Prado (2018) even shows that it is possible to achieve any Sharpe ratio as long as the backtest is repeated enough times.

To avoid artificially inflating the Sharpe ratio, it's important to consider the number of backtests performed and correct for this factor. Additionally, to prevent overfitting to a specific past period, the user could generate multiple paths using combinatorial purged cross-validation. More information on generating these paths can be found in Prado (2018).

Additionally, the [statistics](/wiki/bayesian-statistics) below provide information on the key features of the backtest:

**Sharpe Ratio**: A widely-recognized metric, the Sharpe Ratio measures the risk-adjusted return of a strategy. It's the average return earned in excess of the risk-free rate per unit of volatility. A higher Sharpe Ratio indicates that the returns were more consistent and less volatile[2]. It's a favorite because it gives traders an idea of the strategy's return per unit of risk undertaken.

- **Sortino Ratio**: Similar to the Sharpe Ratio, the Sortino Ratio also assesses the risk-adjusted return. However, while the Sharpe Ratio considers total volatility, the Sortino Ratio only accounts for the downside volatility. This distinction makes it more relevant for traders since they're typically more concerned with negative fluctuations[3].
- **Beta**: Beta measures a strategy's sensitivity or correlation to a benchmark (like a market index). A Beta of 1 indicates the strategy moves in tandem with the benchmark, while a Beta greater than 1 suggests more volatility and less than 1 indicates less volatility. Understanding Beta helps traders gauge the systemic risk a particular strategy might introduce[4].
- **Time range**: This refers to the start and end dates of the testing period, which should be long enough to cover various market conditions.
- **Average AUM**: This is the average value of assets under management, taking into account both long and short positions.
- **Capacity**: This measures the maximum AUM required to achieve the desired risk-adjusted performance, with a minimum AUM necessary for proper bet sizing and risk diversification.
- **Leverage**: This measures the borrowing required to achieve the reported performance, and costs must be assigned to it. Leverage is often calculated as the ratio of average dollar position size to average AUM.
- **Maximum dollar position size**: This indicates whether the strategy at times took dollar positions that greatly exceeded the average AUM, with preference given to strategies that rely less on extreme events or outliers.
- **Ratio of longs**: This shows the proportion of bets that involve long positions, with a ratio close to 0.5 preferred for long-short, market neutral strategies.
- **Frequency of bets**: This is the number of bets per year in the backtest, with a bet defined as a sequence of positions on the same side.
- **Average holding period**: This is the average number of days a bet is held, which can vary significantly depending on the strategy's frequency.
- **Annualized turnover**: This measures the ratio of the average dollar amount traded per year to the average annual AUM, and can be high even with a low number of bets.
- **Correlation to underlying**: This is the correlation between strategy returns and the returns of the underlying investment universe, with a significantly positive or negative correlation indicating that the strategy is essentially holding or short-selling the investment universe without adding much value.

Once armed with these metrics, it's crucial to take a holistic approach in interpreting backtest results. Single metrics can be misleading. For instance, a high Sharpe Ratio might seem promising, but if the strategy was only tested in a bull market, its effectiveness during bearish conditions remains unproven.

Moreover, consider the practicality of the results. If a strategy displays stellar returns, but requires trades every few minutes, it may not be feasible for manual traders. Additionally, always scrutinize results that seem too good to be true. Unrealistically high returns could be a sign of overfitting, where the strategy is too closely tailored to the dataset and might perform poorly in real-world scenarios.

It's also wise to examine drawdowns. A strategy might boast high returns but suffer from large drawdowns (declines in asset value). Large drawdowns can be psychologically taxing for traders and might result in deviating from the strategy during its implementation.

In essence, while metrics like the Sharpe Ratio, Sortino Ratio, and Beta provide valuable insights, they must be contextualized. Consider the broader market conditions, the feasibility of the strategy, and potential psychological impacts. Only by comprehensively evaluating and interpreting these metrics within a larger framework can traders confidently and successfully apply backtested strategies to live trading scenarios.

## Comparative Analysis

Backtesting is a cornerstone of strategy validation, but it isn't the only method traders employ. A well-rounded understanding of how backtesting compares to other testing techniques is crucial.

Here are the most common simulation tools. These are too well known to use space here, so I just give pointers to each and recommend you to google them.

| Test | Run Time | Setup Time | Completeness | Good For |
| --- | --- | --- | --- | --- |
| Backtest | Long | Long | Good | Everything |
| Event Study | Medium | Medium | Good | News |
| Correlation | Fast | Fast | Bad | Prototyping |
| Paper Trading | Live | None | Good | Production Testing |

**Backtest**

Backtesting is simulating a strategy on historic data and looking at the PnL curve at the end. Basically you run the strategy like normal, but the data comes from a historical file and time goes as fast as the computer can process.

**Event Study**

In an event study, you find all the points in time that you have a signal and then average the proceeding and preceding return paths. This shows you on average what happens before and after. You can see how alpha accumulates over time and if there is information leakage before the event.

**Correlation**

The correlation of a signal with future returns is a quick measure of how accuately it predicts. It is better than a backtest when you need just a single number to compare strategies, such as for plotting an information horizon. You can configure a lagged correlation test in Excel in under a minute. However it doesn’t take into account transaction costs, and it doesn’t output trading-relevant metrics like Sharpe ratio or drawdown.

The information horizon diagram was published in Grinold and Kahn’s Active Portfolio Management. It is a principled way of determining how long to hold positions.

**Paper Trading**

Paper trading refers to trading a strategy through your broker’s API, but using a demo account with fake money. It’s good because you can see that the API works, and see if it crashes or if there are data errors. And it also gives you a better feel for the number of trades it will make and how it will feel emotionally. However it takes a long time since you have to wait for the markets. It is more practical for [high frequency](/wiki/high-frequency-trading) systems which can generate a statistically significant number of data points in a short amount of time.

## Potential Pitfalls and How to Avoid Them

Backtesting, while invaluable, is riddled with potential pitfalls that can mislead even seasoned traders. Awareness and understanding of these challenges are the first steps to sidestepping them. Here's a deep dive into some common missteps and strategies to mitigate them.

**Timetravel**

When you are testing a strategy on historical data, you have the ability to give it access to more knowledge than it could possibly have had at that point, like predicting sports with an almanac from the future. Of course it would be dumb to do that, since it is unrealistic, but usually it is accidental. It is not always easy to notice. If you have a strategy that gives a Sharpe over 3 or so on the first test, you should check very carefully that you are not accidentally introducing omniscience. For example, if you use lagged correlation to test a 6-period moving average crossover trend-following strategy and use the moving average through time T to predict time T itself, then you will get a high, but not unreasonable correlation, like .32. It is a hard error to catch and will make your results during live trading quite disappointing.

**Survivorship Bias**

If you test a strategy on all the companies in the S&P500 using their prices over the last 10 years, your backtest results will be biased. Long-only strategies will have higher returns and short-only will have worse returns, because the companies that went bankrupt have disappeared from the data set. Even companies whose market capitalizations decreased because their prices fell will be missing. You need a data source that includes companies’ records even after they have gone bankrupt or delisted. Or you need to think very carefully about the strategy you are testing to make sure it is not susceptible to this bias. For an independent trader, the latter is more practical.

**Adverse Selection**

When executing using limit orders, you will only get filled when someone thinks it will be profitable to trade at your price. That means every position is slightly more likely to move against you than you may have assumed in simulation.

**Instantaneous Communication**

It is impossible to trade on a price right when you see it, although this is a common implementation for a backtester. This is mainly a problem for high-frequency systems where communication latency is not negligible relative to holding periods.

**Transaction Costs**

It is also easy to inaccurately estimate transaction costs. Transaction costs change over time, for example increasing when [volatility](/wiki/volatility-trading-strategies) rises and market makers get scared. Market impact also depends on the [liquidity](/wiki/liquidity-risk-premium) of the stock, with microcaps being the least liquid.

**Unrealistic Backtesting**

There are other issues that sometimes cause problems up but are less universal. For example, your data might not be high enough resolution to show precisely how the strategy will perform. Another problem is if the exchange does not provide enough data to perfectly reconstruct the book (eg the CME).

To fortify your backtesting:

1. Regularly cross-check results using out-of-sample data.
2. Be critical and consistently question the feasibility of your strategies.
3. Keep abreast of market changes and adjust strategies accordingly.
4. Use robust data sources that provide a comprehensive historical view, free from biases.

Armed with this awareness, traders can navigate the intricacies of backtesting more confidently and effectively, developing strategies that stand a greater chance of success in real-world applications.

## Advanced Backtesting Concepts

### Backtesting with cross validation

In machine learning, cross-validation is used to assess how well models generalize over unseen data by splitting the training dataset into parts: a train part to train the model, and a validation part to assess the model on unseen data. Time-series models are prone to overfitting, making cross-validation crucial in estimating the degree of overfitting.

However, standard k-fold cross-validation assumes that data is drawn from an independent and identically distributed stochastic process, which is violated in time-series modeling due to serial correlation. This leads to information leakage between the folds, where information from the training set leaks into the validation set, resulting in an overestimation of the model's performance on unseen data.

To address this, Prado (2018) developed a more robust cross-validation scheme called Combinatorial Purged Cross Validation, which is similar to k-fold but accounts for information leakage. This method purges and embargoes (removes) samples from the train set that are close to the validation set to prevent information leakage, resulting in better estimates of the model's performance on unseen data.

### Optimization

After developing a strategy and backtesting it, most people try to optimize it. This usually consists of tweaking a parameter, re-running the backtest, keeping the result if the results are better, and repeating multiple times.

If you think about backtesting a strategy, you can see how it could be represented as a function:

```python
profit = backtest_strategy(parameter_1, parameter_2, ...)
```

Looking at it this way, it is easy to see how to make the computer test all the possible parameter values for you. Usually it is best to list all the values you want to test for a parameter and try them all (called **brute force** or **grid search**) rather than to try to save computation time using hill-climbing, simulated annealing, or a genetic algo optimizer.

With **hill climbing**, you start with a certain parameter value. Then you tweak it by adding a little or
subtracting a little. If it’s an improvement, keep adding until it stops improving. If it’s worsened, then try subtracting a little and keep subtracting until it stops improving.

**Simulated annealing** adds one feature to hill climbing. After finding a point where no parameter changes will help, in simulated annealing you add some random amount to the parameter value and see if it improves from there. This can help “jump” out of a locally optimal parameter setting, which hill climbing would get stuck in.

**Genetic algo** optimizers add three features. First they run multiple simulated annealings at once with different initial parameter values. The second feature only applies to strategies with multiple parameters. The genetic algo periodically stops the set of simulated annealing algos, and creates new ones by combining subsets of different algo’s parameters. Then it throws away the ones with the least profitable parameter values and starts extra copies of the most profitable ones. Finally, it creates copies that take a little bit from each of two profitable ones. (note: the hill climbing feature is renamed “natural selection,” the simulated annealing feature is renamed “mutation,” the parameter sets are renamed “DNA,” and the sharing feature is called “crossover”).

Let’s see how each of these optimizers looks in a diagram. First, think of the arguments to:

```python
profit = backtest_strategy(parameter_1, parameter_2, ...)
```

as decimal numbers written in a vector:

`|X_1|X_2|X_3|X_4|X_5|X_6|... | ==> $Y`

Let’s say each X variable is in the range -10 to 10. Let’s say there are only two X variables. Then the brute
force approach would be (assuming you cut X’s range up into 3 points):

```python
| X_1 | X_2 | ==> $Y
| -10 | -10 | ==> $5
| -10 |  0  | ==> $6 best
| -10 |  10 | ==> $5
|  0  | -10 | ==> $4
|  0  |  0  | ==> $5
|  0  |  10 | ==> $3
|  10 | -10 | ==> $3
|  10 |  0  | ==> $3
|  10 |  10 | ==> $3
```

The best point is at (-10,0) so you would take those parameter values. This had 32 combinations we had to backtest. But let’s say you have 10 parameters. Then there are 310 ≈ 60, 000 combinations and you will waste a lot of time waiting for it to finish.

Hill climbing will proceed like the following. With hill climbing you have to pick a starting point, which we will say is (0,0), right in the middle of the parameter space. Also we will now change the step size to 5 instead of 10 since we know this optimizer is more efficient.

```
|  0  |  0  |  ==>  $ 5
|  5  |  0  |  ==>  $ 4     worse, try other direction
| -5  |  0  |  ==>  $ 5.5   better, try another step
| -10 |  0  |  ==>  $ 6     better, cannot try another step since at -10
                                    try other variable
| -10 |  5  |  ==>  $ 5.5   worse, try other direction
| -10 | -5  |  ==>  $ 5.5   worse, stop since no other steps to try
```

This only took 6 backtests to find the peak.

Simulated annealing is similar, but adds random jumps. We will choose to do up to 2 random jumps without profit improvement before stopping.

```
|  0  |  0  |  ==>  $ 5
|  5  |  0  |  ==>  $ 4     worse, try other direction
| -5  |  0  |  ==>  $ 5.5   better, try another step
| -10 |  0  |  ==>  $ 6     better, cannot try another step since at -10
                                    try other variable
| -10 |  5  |  ==>  $ 5.5   worse, try other direction

-----^^- above here is same as before -^^-----
| -10 | -5  |  ==>  $ 5.5   worse, try random jump
| -9  |  0  |  ==>  $ 6.1   better, try another random jump
| -9  |  2  |  ==>  $ 6     worse, try another random jump
| -9  |  3  |  ==>  $ 6     worse, stop after some arbitrary

```

It came up with a slightly higher optimal point and took 9 runs of the backtester. Although this is as slow as the brute force approach on this toy example, when you have more parameters, the gains increase.

Now for the genetic optimizer. Use 3 initial members of the population at (-10,-10), (-10,10), and (10,0) to start them as far apart in the space as possible. Run for 3 generations.

```python
         1
| -10 | -10 | ==> $5

    keep 1
| -10 | -10 | ==> $5

    keep 2
| -10 |  0  | ==> $6
        |
         \- best
```

```
         2
| -10 | 10 | ==> $5

crossover X1 on 1 with X2 on 3
| -10 | 0  | ==> $6

    keep but mutate 2
| -10 | 2  | ==> $5.7
```

```
         3
|  10 | 0 | ==> $3

keep but mutate 2
| -10 | 8 | ==> $5.1

keep but mutate 3
| -10 | 9 | ==> $5
```

By pure luck, crossover placed us right at the optimal parameters in this example. This also took 9 backtests. It also required the overhead of crossover and mutation. Genetic algorithms are often significantly slower than simulated annealing, though in theory they are faster than brute force.

In general these fancy optimizers are overkill and can create hard to detect problems. In trading it’s better to have fewer parameters than many. It is best to test all the possible values of a parameter and plot the graph of profits vs parameter value. If the optimizer has found a parameter value that is at an isolated peak on the curve, you are probably overfitting.

Here is an example of a profitability curve for an imaginary strategy with one parameter, an exponential moving average’s length:

![Screenshot 2023-03-18 at 15.42.52.png](images/Screenshot_2023-03-18_at_15.42.52.png)

Here there aren’t any potential overfitting points, however there is a local maximum at EMA length of 1 which could mess up the hill climbing optimizers. Overfitting is often presented as a curse that one must carefully ward off with rituals and sacrificial stress testing simulations. However typically (at least when not using fancy machine learning algos like SVMs or neural nets) it appears in intuitive places. For example with a moving average convergance-divergance momentum strategy, overfitting will typically rear its ugly head when the two MA lengths are almost equal, or when one or both is very low (eg 1, 2, 3, or 4ish bars). This is because you can catch a lot of quick little market turns if the market happened to be trading a the perfect speed during a perfect little time period [in the past].

### Bet sizing

Building a trading strategy using a model that predicts the side of the trade is useful, but opening the position with a fixed size can be inefficient. A better way to size the position would be to use the model's confidence in its prediction. This concept is called bet sizing, and the following sections will explain it further.

When metalabeling is applied on top of a primary model that predicts the side of the trade, the metalabeling model outputs a predicted probability that can be used to determine the position size. The metalabeling model is a binary classifier that predicts whether to take or not take the trade.

The goal is to test the null hypothesis $H_0$: $p[x =1] = \dfrac{1}{2}$, where $p[x = 1]$ is the probability whether the side is correct and $x \in \{-1, 1\}$, where -1 and 1 represents short and long respectively. The test statistic $z$ is defined as

$$
z = \dfrac{p[x=1] - \dfrac{1}{2}}{\sqrt{p[x=1](1-p[x=1])}} \sim \mathcal{N}(0, 1), z \in (-\infty, \infty)
$$

when the metalabelling model predicts $p[x=1]$, we compute the $z$ test statistic, which we can put into the CDF of the standard normal distribution to get a bet size. However, this can lead to excessive trading with small amounts when the predicted probability $p[x=1]$ is close to 0.5. To filter out these noisy trades, we can discretise the CDF in steps such that probabilities close 0.5, are floored to a size of 0.

### Backtesting on synthetic data

Each strategy has an implementation tactic called "trading rules," which provide the algorithm to enter and [exit](/wiki/exit-strategy) a position. These rules rely on historical simulations, which can lead to the problem of backtest overfitting, making the investment strategy unfit for the future.

The goal is to exit a position optimally, which is a dilemma often faced by execution traders, and it should not be confused with the determination of entry and exit thresholds for investing in a security. To avoid the risk of overfitting, a good practice is deriving the optimal parameters for the trading rule directly from the stochastic process that generates the data, rather than engaging in historical simulations.

You can:

- construct a mesh of stop-loss and profit-taking pairs,
- generate paths for prices,
- apply the stop-loss and profit-taking logic,

and determine the optimal trading rule within the mesh. This approach avoids the problem of backtest overfitting and is applicable to various specifications, such as the discrete Ornstein-Uhlenbeck process on prices. Examples of financial data that can be generated include stock prices, stock returns, correlation matrices, retail banking data, and all kinds of market microstructure data.

## The Next Steps After Backtesting

Once backtesting has provided insight into a strategy's historical performance, the subsequent move is to translate this knowledge into real-world trading. This journey is often denoted as transitioning from paper trading (or simulated trading) to live trading.

Paper trading allows traders to simulate real trading scenarios without risking actual capital. It’s an invaluable phase that helps in gaining familiarity with trading platforms, order placements, and the strategy's practicality. However, paper trading lacks the psychological pressures of real money at stake, which can influence decision-making[5].

Transitioning from paper trade to live trade requires a structured approach. Start small: this isn't about hitting home runs immediately but understanding the nuances of live trading conditions and adapting the strategy accordingly. Real markets are dynamic and can exhibit behavior that wasn’t present or visible during the backtesting phase.

Even after moving to live trading, it’s imperative to consider it an iterative process. Continuous monitoring is non-negotiable. Every strategy, no matter how robust, will have its periods of underperformance. The key is to discern between natural drawdowns (part of the strategy) and systemic changes in the market rendering the strategy ineffective.

Optimization, although valuable, comes with its pitfalls. If done excessively, it can lead to overfitting, where a strategy performs well on past data but poorly in real-time trading. The trick is to strike a balance: regularly review the strategy's performance against its historical metrics but be cautious of making frequent tweaks based solely on short-term results.

In conclusion, the journey from backtesting to live trading is one of adaptation, vigilance, and refinement. While backtesting provides a foundation, the real test of a strategy's mettle occurs in the tumultuous waters of live markets. And as always, ongoing education, diligence, and risk management remain the trader's best allies.

## Conclusion

Backtesting remains a cornerstone in trading, offering traders an invaluable lens to gauge the potential of their strategies. By simulating how a strategy would have performed using historical data, backtesting provides insights into its strengths, weaknesses, and potential risks. Yet, while it's an essential tool, it's only part of the equation in crafting a successful trading career.

While the allure of a well-performing backtested strategy can be enticing, it's paramount to approach live trading with the same rigor and diligence. Financial markets are intricate ecosystems, continuously evolving and influenced by myriad factors. What worked in the past might not necessarily guarantee success in the future.

Thus, while backtesting offers a solid foundation, real trading is where theory meets practice. Always remember to tread with caution, continuously educate oneself, and ensure a steadfast commitment to risk management. Implementing the insights from backtesting can pave the way for trading success, but it requires both knowledge and prudence in equal measure.

## References & Further Reading

[1]: Chan, E. P. (2008). [Quantitative trading: How to build your own algorithmic trading business](https://www.amazon.com/Quantitative-Trading-Build-Algorithmic-Business/dp/0470284889). John Wiley & Sons.

[2]: [Understanding the Sharpe Ratio](https://www.investopedia.com/terms/s/sharperatio.asp) - Investopedia.

[3]: [The Sortino Ratio: A Better Measure of Risk](https://www.investopedia.com/terms/s/sortinoratio.asp) - Investopedia.

[4]: [Beta: Know the Stock's Risk Profile](https://www.investopedia.com/investing/beta-know-risk/) - Investopedia.

[5]: [The Importance of Paper Trading](https://www.investopedia.com/terms/p/papertrade.asp) - Investopedia.