---
title: "Backtesting.py Guide (Algo Trading)"
description: Discover how backtesting enhances algorithmic trading by using historical data to assess trading strategies before real-world application. Learn about Python's role in streamlining this process with its user-friendly syntax and powerful libraries for data manipulation and visualization. This guide covers the essentials of backtesting, the advantages of Python, strategy development steps, and transitioning from simulation to live trading, offering insights into maximizing trading success while minimizing risk.
---





Backtesting is a crucial component of algorithmic trading, allowing traders to evaluate the viability and effectiveness of a trading strategy using historical data before deploying it in real market conditions. This process serves as a simulation where past data is used to test if a specific strategy would have been successful, providing traders with insights into potential future performance. Its primary purpose is to reduce risks and increase the probability of trading success by identifying and fine-tuning strategies prior to their live application.

Python has emerged as a popular choice for backtesting due to several factors. Its ease of use and readable syntax make it accessible to both novice and experienced programmers, encouraging a wider adoption across various levels of expertise. Python's comprehensive ecosystem of libraries, specifically geared toward finance and data analysis, such as pandas, NumPy, and matplotlib, provide users with the tools needed to efficiently manipulate data and visualize results. Furthermore, Python's flexibility allows for the development of entire end-to-end trading systems, integrating backtesting with strategy development, optimization, and execution.

This article is structured to guide readers through the significance and practical application of backtesting in algorithmic trading. It begins with an explanation of backtesting, followed by the advantages of using Python, a review of essential Python libraries, a step-by-step guide to backtesting, and a discussion on advanced techniques and common pitfalls. Finally, it explores the transition from backtests to live trading, supplemented with case studies of successful implementations.

Before deploying a trading strategy, backtesting provides numerous benefits. It helps in understanding the strategy's historical performance, identifying weaknesses, and addressing them before they result in financial losses in live trading. Backtesting also quantifies the strategy's risk and reward profile, allowing traders to make informed decisions based on performance metrics like the Sharpe ratio, maximum drawdown, and annualized return.

The accuracy of backtesting directly correlates with trading success. An accurate backtest accounts for various factors such as transaction costs, market slippage, and changes in market conditions, ensuring that the simulation closely mirrors real-world trading. However, traders must be cautious of overfitting, where a strategy is excessively tailored to historical data, potentially leading to poor performance when applied to unseen data. By maintaining rigorous standards of data quality and realistic assumptions, traders can significantly enhance the reliability of their backtesting efforts, paving the way for more successful algorithmic trading.


## Table of Contents

## Understanding Backtesting in Algorithmic Trading

Backtesting is a critical component of algorithmic trading, allowing traders to evaluate the viability of a trading strategy by applying it to historical market data. The fundamental purpose of backtesting is to estimate how a trading strategy would have performed in the past, thereby providing insights into its potential future performance. This process helps traders identify profitable strategies, assess risk, and optimize parameters before committing capital in live markets.

The [backtesting](/wiki/backtesting) process involves running a trading strategy on historical data to create a simulated trading environment. Traders can thus determine how a strategy would have performed based on actual past price movements, without any financial risk. During backtesting, strategies are typically executed using a software that can handle massive datasets and complex calculations—an area where Python excels due to its efficient processing capabilities and extensive libraries.

Key terms associated with backtesting include:

- **Historical data**: Past market data, such as prices, volumes, and order book information, used to simulate trades. The quality and granularity of this data directly influence the validity of backtesting results.
- **Strategy**: A predefined set of rules governing entry, exit, and position-sizing in trading. These rules can be based on technical indicators, price patterns, or other market signals.
- **Simulation**: The process of executing trades using a strategy on historical data to evaluate potential performance.
- **Metrics**: Performance indicators used to assess the efficiency and risk of a trading strategy. Common metrics include return on investment (ROI), Sharpe ratio, maximum drawdown, and win-to-loss ratio.

Several challenges accompany backtesting, with data quality being one of the most significant. Inaccurate or incomplete data can lead to unreliable results. Traders must ensure that the historical data used is clean, accurate, and relevant to the markets they intend to trade. Additionally, adjusting for factors such as corporate actions and dividend adjustments is essential for stocks.

Another common challenge is the **look-ahead bias**, which occurs when a strategy inadvertently uses information that would not have been available at the time of trading. To mitigate this, it is imperative that traders carefully design their simulation to prevent future data from influencing past events.

An effective backtesting approach addresses these issues through rigorous data handling and strategy validation. This not only refines and enhances trading strategies but also improves the likelihood of success in live trading environments.


## Advantages of Using Python for Backtesting

Python has become a predominant language in backtesting for [algorithmic trading](/wiki/algorithmic-trading) due to its ease of use, readability, and expansive ecosystem. These features make it an attractive option for both novice and experienced traders seeking to develop and refine trading strategies.

### Ease of Use and Readability

Python’s syntax is designed to be clean and easy to understand, making it accessible to programmers and non-programmers alike. The language's readability enables users to easily follow the logic of a trading strategy, which is critical when ensuring accuracy in backtesting. Python allows for rapid prototyping, testing, and iteration of ideas, which is crucial in the fast-paced and competitive world of trading. The language's intuitive structure reduces the learning curve, allowing traders to focus more on strategy development and less on coding complexities.

### Rich Ecosystem of Libraries

One of Python's most significant advantages is its vast ecosystem of libraries. Libraries such as Pandas and NumPy provide robust tools for data manipulation and numerical analysis, essential for processing historical trading data. Visualization libraries like Matplotlib and Seaborn allow traders to create detailed graphics to analyze backtest results visually.

Specialized libraries like Backtrader, PyAlgoTrade, and Zipline are specifically designed for algorithmic trading backtesting. These libraries provide a framework for developing and testing trading strategies, complete with features for handling large datasets, optimizing strategies, and generating detailed performance reports. This wealth of resources significantly reduces the time and effort required to implement effective backtesting routines.

### Community Support and Resources

Python boasts a large and active community, which results in a wealth of shared knowledge and freely available resources. This community-driven support is invaluable for troubleshooting, learning best practices, and accessing cutting-edge techniques in algorithmic trading. Online forums, tutorials, and documentation ensure that traders can find solutions to their problems and stay informed about the latest advancements and methodologies.

### Versatility for Full-Fledged Trading Systems

Beyond backtesting, Python’s versatility extends to building complete trading systems. Python can be integrated with various APIs and brokers, facilitating a seamless transition from strategy development to live trading execution. It supports computationally intensive tasks, enabling the incorporation of [machine learning](/wiki/machine-learning) models, advanced statistical analyses, and real-time data processing.

The combination of portability, flexibility, and comprehensive library support ensures that Python is not only a tool for backtesting but is also suited for the entire trading lifecycle. Its capability to interface with other programming languages and databases makes it an ideal choice for traders who require a customized and scalable trading infrastructure.

In summary, Python's ease of use, extensive library ecosystem, and strong community make it an ideal language for backtesting in algorithmic trading. Its ability to handle complex data analyses and integrate into full trading systems underscores its position as a critical tool for traders aiming to enhance and execute strategies effectively.


## Essential Python Libraries for Backtesting

Python has become a cornerstone in the field of algorithmic trading, largely due to its comprehensive suite of libraries that facilitate backtesting—a critical component for evaluating trading strategies. This section highlights the essential Python libraries widely employed in backtesting, providing insights into their functionalities and applications.

**1. Key Libraries: Pandas, NumPy, Matplotlib**

The trio of Pandas, NumPy, and Matplotlib forms the backbone of data manipulation, numerical analysis, and data visualization in Python.

- **Pandas**: This library is crucial for handling time-series data, often used in financial datasets. Its `DataFrame` and `Series` structures allow for efficient data manipulation, filtering, and aggregation. It simplifies operations such as resampling and rolling computations, essential for calculating moving averages or other indicators.

- **NumPy**: Known for its performance, NumPy provides support for large multi-dimensional arrays and matrices, along with a rich collection of mathematical functions. It facilitates fast computational operations on arrays, which is useful for simulations and performance-sensitive calculations.

- **Matplotlib**: As a plotting library, Matplotlib is employed to create static, interactive, and animated visualizations. It is frequently used to plot price movements, trading signals, and backtest results, helping traders better understand strategy performance.

**2. Specialized Libraries: Backtrader, PyAlgoTrade, Zipline**

Unlike more general-purpose libraries, these specialized tools are designed specifically for financial backtesting and analysis.

- **Backtrader**: Renowned for its versatility and simplicity, Backtrader supports multiple data feeds and strategies. It offers features such as strategy optimization, walk-forward analysis, and support for live trading, making it a comprehensive platform for both beginners and experienced traders.

- **PyAlgoTrade**: This library is tailored for simplicity and performance. It allows users to easily develop and test algorithmic trading strategies. While its feature set is not as extensive as Backtrader, it is well-suited for users who require a straightforward tool to test their trading hypotheses.

- **Zipline**: Developed by Quantopian, Zipline is an open-source library that powers Quantopian’s system. It is ideal for complex backtesting due to its event-driven architecture and built-in analysis functionalities. Its integration with Quantopian’s IDE (when it was operational) further extended its capabilities through community collaboration.

**3. Comparison with Other Programming Languages and Tools**

In algorithmic trading, the decision on which technology stack to employ can significantly impact development and execution efficiency. While languages like C++ and Java offer speed, Python's simplicity and ease of learning make it highly accessible. Compared to R, another popular choice in the finance industry, Python offers broader integrations with web and database tools, making it ideal for end-to-end trading systems.

**4. Best Practices for Selecting a Library Based on Strategy Complexity**

When selecting a library for backtesting, consider the following best practices:

- **Level of Complexity**: For simple strategies, Pandas combined with NumPy for custom calculations might suffice. More complex strategies involving multiple securities, risk management, and order handling may benefit from specialized platforms like Backtrader or Zipline.

- **Performance Needs**: NumPy and Cython can optimize performance-critical parts of the code. In cases where speed is paramount (e.g., high-frequency trading), integrating C++ code or using libraries focused on speed, such as Numba, can be beneficial.

- **Community and Documentation**: Large and active communities can provide support and a wealth of shared knowledge. Libraries with comprehensive documentation and tutorials are easier to adopt and integrate.

In conclusion, leveraging Python's rich ecosystem of libraries can significantly streamline the development of robust backtesting solutions, facilitating better strategic decisions in algorithmic trading.


## Step-by-Step Guide to Backtesting with Python

To effectively backtest a trading strategy using Python, it's crucial to follow a structured approach that includes setting up the environment, acquiring data, implementing a strategy, and interpreting results. This guide outlines the key steps involved in performing a backtest with the Python programming language and the Backtrader library.

### Setting Up Your Python Environment

Begin by installing Python and necessary libraries. A recommended setup includes Python 3.x and a package manager like pip. Essential packages for backtesting include:

- **pandas** for data manipulation and analysis
- **NumPy** for numerical computations
- **matplotlib** for plotting
- **Backtrader** for executing backtests

You can install these packages using pip:

```bash
pip install pandas numpy matplotlib backtrader
```

### Gathering and Preparing Historical Data

Data is the backbone of backtesting. Historical price data can be sourced from financial data providers such as Alpha Vantage, QuantConnect, or Yahoo Finance. The data should ideally include timestamps, open, high, low, close prices, and [volume](/wiki/volume-trading-strategy). Ensure that the data is cleaned and formatted correctly:

```python
import pandas as pd

# Example of reading CSV file containing historical data
data = pd.read_csv('historical_data.csv', index_col='Date', parse_dates=True)
```

### Developing a Simple Trading Strategy

A trading strategy outlines the rules for entering and exiting trades. A simple example is a moving average crossover strategy, where trades are executed based on the crossover of short-term and long-term moving averages:

```python
class MyStrategy(bt.Strategy):
    params = (('short_period', 20), ('long_period', 50),)
    
    def __init__(self):
        self.short_mavg = bt.indicators.SimpleMovingAverage(self.data.close, period=self.params.short_period)
        self.long_mavg = bt.indicators.SimpleMovingAverage(self.data.close, period=self.params.long_period)

    def next(self):
        if self.short_mavg > self.long_mavg and not self.position:
            self.buy()
        elif self.short_mavg < self.long_mavg and self.position:
            self.sell()
```

### Performing the Backtest Using Backtrader

Backtrader simplifies the execution of backtests. To perform a backtest, set up a `Cerebro` engine, add the strategy, and supply the historical data:

```python
import backtrader as bt

# Initialize the Cerebro engine
cerebro = bt.Cerebro()
cerebro.addstrategy(MyStrategy)

# Add the data feed to Cerebro
data_feed = bt.feeds.PandasData(dataname=data)
cerebro.adddata(data_feed)

# Run the backtest
initial_cash = 10000
cerebro.broker.setcash(initial_cash)
cerebro.run()

# Plot the results
cerebro.plot()
```

### Analyzing Backtest Results and Interpreting Performance Metrics

After conducting a backtest, analyzing the results is crucial for understanding the performance of the strategy. Key metrics to evaluate include:

- **Net profit or loss:** Final portfolio value minus the initial investment.
- **Sharpe Ratio:** A measure of risk-adjusted return, calculated as $(\text{mean return - risk-free rate}) / \text{standard deviation of returns}$.
- **Maximum drawdown:** The peak-to-trough decline during a specific period, indicating the risk of a strategy.

Backtrader provides built-in analyzers to gather these metrics:

```python
final_cash = cerebro.broker.getvalue()
print(f"Final Portfolio Value: {final_cash}")

# Add analyzers to get performance metrics
cerebro.addanalyzer(bt.analyzers.SharpeRatio, _name='sharpe')
result = cerebro.run()
sharpe_ratio = result[0].analyzers.sharpe.get_analysis()
print(f"Sharpe Ratio: {sharpe_ratio['sharperatio']}")
```

Interpreting these metrics assists in assessing the feasibility and potential adjustments needed for a trading strategy before it is transitioned to live trading conditions. Proper analysis ensures that the strategy can withstand market volatilities while delivering respectable returns.


## Advanced Techniques in Python Backtesting

In algorithmic trading, refining strategies using advanced techniques in Python can significantly enhance the robustness and reliability of the systems being developed. This section explores several key methodologies: Monte Carlo simulations, walk-forward optimization, the incorporation of machine learning models, and adjustments for transaction costs and slippage.

### Monte Carlo Simulations 

Monte Carlo simulations are used to assess the robustness of a trading strategy by generating a range of possible performance outcomes. By simulating a multitude of trades under varying conditions, traders can evaluate the effects of randomness and non-ideal market scenarios on their strategies. The process involves altering input variables within realistic bounds and running the strategy across these permutations. In Python, this can be achieved using libraries such as NumPy for random number generation and pandas for data manipulation.

**Python Example:**

```python
import numpy as np

# Simulate strategy returns
def monte_carlo_simulation(returns, num_simulations):
    simulations = []
    for _ in range(num_simulations):
        np.random.shuffle(returns)
        simulations.append(np.mean(returns))
    return np.percentile(simulations, [5, 95])  # 5th and 95th percentile

historical_returns = np.random.normal(0, 1, 100)  # Example returns
mc_result = monte_carlo_simulation(historical_returns, 1000)
```

### Walk-Forward Optimization 

Walk-forward optimization is a strategy validation method that extends simple backtesting by continuously optimizing the parameters of a trading strategy and testing it on subsequent out-of-sample data. This technique addresses overfitting by dividing historical data into multiple segments, performing parameter optimization on each segment, and testing these parameters on the data immediately following each segment.

**Python Approach:**

1. Divide data into training and testing segments.
2. Optimize strategy parameters on the training set.
3. Validate strategy on the immediately following test set.

### Integrating Machine Learning Models

Machine learning models provide powerful capabilities for pattern recognition and predictive analytics in trading strategies. Models such as decision trees, neural networks, and support vector machines can be integrated into strategies to predict market movements or classify trading signals. Python’s scikit-learn and TensorFlow are prominent libraries offering robust tools for machine learning applications. When utilizing these models, it is crucial to separate training and validation data to mitigate the risk of overfitting.

**Example with Scikit-learn:**

```python
from sklearn.ensemble import RandomForestClassifier
from sklearn.model_selection import train_test_split

features, labels = # data preparation phase
X_train, X_test, y_train, y_test = train_test_split(features, labels, test_size=0.2)

model = RandomForestClassifier(n_estimators=100)
model.fit(X_train, y_train)
accuracy = model.score(X_test, y_test)
```

### Adjusting for Transaction Costs and Slippage

Adjusting backtest results for transaction costs and slippage is essential for obtaining realistic outcomes. Transaction costs include broker fees and market impact, while slippage refers to the difference between the expected price of a trade and the actual price. This can dramatically affect a strategy’s profitability. When modeling slippage and transaction costs, it’s beneficial to assume conservative estimates to avoid optimistic bias.

**Practices:**

- Deduct fixed and variable transaction costs from each trade in the backtest.
- Apply a slippage model, perhaps scaling with volatility, to order execution prices.

Fulfilling these advanced methodological considerations will better equip algorithmic traders to develop, validate, and enhance their trading systems within Python, optimizing for real-world performance and risk management.


## Common Pitfalls in Backtesting and How to Avoid Them

Backtesting is a critical step in the development of any algorithmic trading strategy, yet it presents several pitfalls that traders must watch for to ensure robust results. Understanding and avoiding these common issues can significantly improve the reliability of backtest outcomes and, ultimately, the success of live trading.

### Understanding and Avoiding Curve Fitting

Curve fitting, or overfitting, occurs when a trading strategy is too closely tailored to historical data, capturing noise rather than the underlying market dynamics. This can result in a strategy that performs well on past data but poorly in live markets. 

To avoid curve fitting, adhere to the following practices:

- **Simplicity**: Keep the model as simple as possible. Complex models with numerous parameters are more prone to curve fitting.
- **Training and Validation Split**: Divide your historical data into separate training and validation sets. Develop your strategy on the training set and validate its performance on the unseen data.
- **Regularization Techniques**: Use regularization methods that constrain or penalize model complexity, such as L1 or L2 regularization in machine learning frameworks.

### Handling Data Snooping Bias

Data snooping bias arises when repeated use of the same dataset leads to overly optimistic estimates of a strategy's performance. This can occur when a strategy is continuously adjusted to improve backtest outcomes without independent validation.

To mitigate data snooping bias:

- **Out-of-Sample Testing**: After developing a strategy on a particular dataset, test it on completely new, out-of-sample data to assess its true predictive power.
- **Cross-Validation**: Employ cross-validation methods where applicable, rotating through multiple data segments to ensure consistent performance.
- **Blind Rule Formulation**: Define trading rules before examining the data. This prevents the creation of rules that are inadvertently tailored to historical patterns.

### Importance of Realistic Assumptions Regarding Market Conditions

Accurate assumptions about transaction costs, slippage, and [liquidity](/wiki/liquidity-risk-premium) are vital in creating realistic backtests. Neglecting these aspects can lead to inflated performance metrics.

To incorporate realistic assumptions:

- **Transaction Costs**: Account for all trading fees, including broker commissions and any platform fees.
- **Slippage**: Implement slippage models that simulate the cost of executing trades at prices different from the trading signals, owing to market movements.
- **Liquidity Constraints**: Ensure that your strategy can be executed in real market conditions, accounting for the volume and volatility of the assets being traded.

### Validating a Strategy Outside of Backtesting Results

A strategy's effectiveness cannot solely rely on backtest results. Real-world validation is crucial for gauging its viability.

Validation methods include:

- **Paper Trading**: Engage in paper trading to simulate real trading without involving actual capital. This helps in understanding how a strategy might perform in live markets.
- **Walk-Forward Testing**: Continually re-optimize the strategy over successive periods and test its performance on forward data.
- **Continuous Monitoring**: Even after transitioning to live trading, continuously monitor the strategy's performance, recalibrating and optimizing it as necessary based on current market conditions.

Addressing these common pitfalls in backtesting enhances the likelihood of developing a trading strategy that is robust, reliable, and successful in both simulated and real-world environments.


## Putting It All Together: From Backtesting to Live Trading

Transitioning from backtesting to live trading represents a crucial step in the lifecycle of an algorithmic trading strategy. Thorough backtesting provides a statistically sound basis for confidence in a trading algorithm, yet live trading presents its own unique challenges that must be addressed.

### Transitioning from Backtests to Live Execution

The move from backtesting to live execution necessitates consideration of multiple factors, including market liquidity, latency, and transaction costs, which might not be fully captured during the backtest. Ensuring that a strategy performs as expected involves rigorous validation and testing in a simulated live environment, often called paper trading. This step allows traders to gauge the algorithm’s performance in real-time without financial risk. A key aspect is the alignment of data used in backtesting with the live data feed to maintain consistency.

### Monitoring a Live Strategy and Continuously Improving It

Once operational, monitoring the live strategy becomes imperative to ensure it achieves expected performance metrics. This involves monitoring key performance indicators (KPIs) such as profit and loss (P&L), Sharpe ratio, and maximum drawdown. Constant vigilance allows traders to identify underperformance early and adjust strategies accordingly. Furthermore, continuous improvement is essential. This could involve recalibrating parameters based on market changes or integrating emerging data to refine predictions and trades.

### Integrating Python Backtesting Frameworks with Brokerage APIs

Python's robust ecosystem offers several libraries like Backtrader, PyAlgoTrade, and Zipline that can be integrated with brokerage APIs. This integration facilitates the live execution of strategies through electronic trading platforms. For instance, using the `[backtrader](/wiki/backtrader)` library with an [Interactive Brokers](/wiki/interactive-brokers-api) API can streamline the transition process. Here's an example of how one might set up a live feed and execute:

```python
import backtrader as bt

class TestStrategy(bt.Strategy):
    def next(self):
        if not self.position:
            self.buy(size=1)
        else:
            self.sell(size=1)

cerebro = bt.Cerebro()
cerebro.addstrategy(TestStrategy)

# Assuming the use of Interactive Brokers as a broker
ibstore = bt.stores.IBStore(port=7496)  # connects to TWS
data = ibstore.getdata(dataname='AAPL-STK-SMART-USD')
cerebro.adddata(data)

cerebro.run()
```

This script demonstrates setting up a simple buy-and-sell strategy using the Interactive Brokers API via Backtrader.

### Case Studies of Successful Transitions

There are numerous case studies that exemplify successful transitions from backtesting to live trading. For example, quantitative hedge funds often use backtesting and subsequent live testing as blueprints. A notable case is the integration of machine learning models, which were first backtested in Python, to capture market anomalies in live trading. Such transitions underscore the importance of a systematic approach, where rigorous backtesting is used to validate hypotheses, which are then iteratively tested in live markets.

In conclusion, bridging the gap from backtesting to live trading requires meticulous preparation and continuous strategy refinement. Utilizing Python’s capabilities, traders can establish a seamless transition, leveraging backtesting insights to optimize real-world trading performance. This ongoing process not only helps in mitigating the risks associated with live trading but also enhances the robustness of trading strategies over time.


## Conclusion

Backtesting holds a vital place in algorithmic trading, providing a framework to evaluate and refine trading strategies before deploying them in the live market. By simulating the application of a strategy on historical data, traders can better understand potential outcomes, risk, and profitability. The process helps to uncover flaws, optimize parameters, and enhance overall strategy performance, thereby increasing the likelihood of success when trading real-time.

Python stands out as an efficient and accessible tool for backtesting. With its ease of use, readability, and a rich ecosystem of libraries tailored for financial analysis, Python facilitates both beginners and seasoned traders in crafting robust backtesting environments. Libraries such as pandas, NumPy, and matplotlib offer powerful capabilities for data manipulation and visualization, while specialized libraries like Backtrader and PyAlgoTrade provide comprehensive features for executing and analyzing backtests with minimal setup.

Practicing and refining backtesting skills is crucial for anyone interested in algorithmic trading. Consistent practice enables traders to develop a keen understanding of the nuances involved in strategy evaluation and optimization. As they become adept at anticipating pitfalls and adjusting their strategies accordingly, traders will find themselves better prepared to transition from simulated to live trading conditions.

For beginners embarking on their backtesting journey, it's essential to start with simple strategies and gradually introduce complexity. This approach allows for building a solid foundation of understanding fundamental concepts before tackling advanced techniques. Paying attention to potential biases such as curve fitting and data snooping is necessary to ensure realistic and reliable backtest results. Finally, engaging with the vibrant Python community can provide valuable resources and support, ultimately fostering growth and proficiency in backtesting endeavors.




## References & Further Reading

[1]: Bergstra, J., Bardenet, R., Bengio, Y., & Kégl, B. (2011). ["Algorithms for Hyper-Parameter Optimization."](https://papers.nips.cc/paper/4443-algorithms-for-hyper-parameter-optimization) Advances in Neural Information Processing Systems 24.

[2]: ["Advances in Financial Machine Learning"](https://www.amazon.com/Advances-Financial-Machine-Learning-Marcos/dp/1119482089) by Marcos Lopez de Prado

[3]: ["Evidence-Based Technical Analysis: Applying the Scientific Method and Statistical Inference to Trading Signals"](https://www.amazon.com/Evidence-Based-Technical-Analysis-Scientific-Statistical/dp/0470008741) by David Aronson

[4]: ["Machine Learning for Algorithmic Trading"](https://github.com/stefan-jansen/machine-learning-for-trading) by Stefan Jansen

[5]: ["Quantitative Trading: How to Build Your Own Algorithmic Trading Business"](https://books.google.com/books/about/Quantitative_Trading.html?id=j70yEAAAQBAJ) by Ernest P. Chan

[6]: ["Python for Algorithmic Trading: From Idea to Cloud Deployment"](https://www.amazon.com/Python-Algorithmic-Trading-Cloud-Deployment/dp/149205335X) by Yves Hilpisch

[7]: ["Python for Data Analysis"](https://wesmckinney.com/book/) by Wes McKinney

[8]: Fama, E. F., & French, K. R. (1992). ["The Cross‐Section of Expected Stock Returns."](https://www.jstor.org/stable/2329112) Journal of Finance, 47(2), 427-465.

[9]: Pojarliev, M., & Levich, R. M. (2010). ["Detecting Crowded Trades in Currency Funds."](https://www.nber.org/papers/w15698) Financial Analysts Journal, 66(2), 26-39.