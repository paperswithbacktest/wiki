---
title: "Momentum"
description: Discover the concept of Momentum in Algorithmic Trading and its significance in capitalizing on existing market trends. Learn about historical context, theoretical explanations, and practical implementations of momentum strategies through technical indicators like Moving Averages (SMA & EMA) and Relative Strength Index (RSI). Explore the evolution of momentum trading from manual to algorithmic practices.
---

Momentum in Algorithmic (Algo) Trading refers to a strategy that capitalizes on the continuance of existing trends in the market. Essentially, it involves leveraging technological algorithms to execute trades aimed at exploiting existing upward or downward trends in asset prices.

The significant role of algo trading in [momentum trading](https://paperswithbacktest.com/paper/optimal-momentum-a-global-cross-asset-approach) lies in its ability to systematically identify, assess, and execute trading opportunities with speed and efficiency, often far surpassing human capabilities.

![Image](images/1.png)

Undertaking a profound comprehension and implementation of momentum in algo trading is pivotal due to its prevailing utilization among hedge funds, institutional traders, and individual investors alike. [Momentum strategies](https://paperswithbacktest.com/paper/momentum-effects-in-country-equity-indexes), when tactically executed via algo trading, can potentially harness significant profits and simultaneously, when paired with prudent risk management strategies, shield the trader from substantial losses.

This article is crafted to explore the multifold aspects of momentum in algo trading, aspiring to enlighten both novice and seasoned traders on its intricate dynamics, historical evolution, practical implementations, and future trajectories.

## Table of Contents

## An In-depth Exploration of Momentum Trading

Momentum, a term borrowed from physics, refers to the quantity of motion an object has. In physics, momentum is often described as the product of an object's mass and velocity. Just as an object in motion tends to stay in motion unless acted upon by an external force, in the world of finance, momentum signifies a trend's strength and its likelihood to continue on its current course.

Transitioning this concept to the financial markets, [momentum](/wiki/momentum) trading seeks to capitalize on existing market trends, buying assets that are trending upward and selling them once they show signs of reversal. This strategy works on the rationale that assets that have ascended in price during recent periods are more likely to continue rising, and those that have descended are likely to keep going down. It's less about the absolute value of an asset and more about its relative movement compared to previous periods and perhaps other assets or market benchmarks.

The momentum phenomenon in financial markets is not a new revelation. A substantial body of academic research attests to its persistence and ubiquity across different markets and time frames. For instance, Jegadeesh and Titman's 1993 study, "Returns to Buying Winners and Selling Losers: Implications for Stock Market Efficiency," presented compelling evidence supporting [momentum-based strategies](https://paperswithbacktest.com/) over 3 to 12-month horizons[1]. Their research found that stocks that performed well over the past 3 to 12 months continued to outperform, while stocks that performed poorly continued to underperform.

From a theoretical perspective, the momentum effect has been attributed to various [factor](/wiki/factor-investing)s, both rational and behavioral. One rational explanation lies in the gradual information diffusion hypothesis, suggesting that not all information reaches all market participants simultaneously[2]. Therefore, price adjustments happen progressively over time, creating momentum. On the behavioral side, cognitive biases, such as investor overconfidence or herding behavior, play a role. Investors might initially underreact to new information, causing a lag in price adjustment, and then overreact as more and more traders follow the trend, propelling prices further in the direction of the trend.

## The Historical Context of Momentum Investing and Trading

One of the earliest recognitions of momentum was by the famed economist, Alfred Cowles, in the 1930s, who identified tendencies of stock prices to continue in their existing direction[3].

In the decades that followed, as financial markets developed and information dissemination became more efficient, the concept of momentum trading expanded. Jesse Livermore, a famed early 20th-century trader, employed what can be seen as momentum strategies, buying stocks as they broke out to new highs and selling when they began to falter. His trading principles, detailed in the book "Reminiscences of a Stock Operator" by Edwin Lefèvre, illuminate the early practices of momentum trading[4].

The late 20th century witnessed an explosion in momentum strategies due to several factors. Firstly, the 1990s technological boom provided traders with more advanced tools for analysis, leading to more sophisticated momentum-based strategies. Secondly, the proliferation of academic studies, like the seminal work by Jegadeesh and Titman in 1993, offered empirical validation to momentum as a viable anomaly in markets[1].

The arrival of the 21st century marked the transition from manual momentum trading practices to algorithmic ones. The advent of high-frequency trading and the increasing computational power allowed traders to execute momentum strategies at unparalleled speeds and accuracy. This new era was marked by influential figures like Cliff Asness, co-founder of AQR Capital Management, who championed factor-based investing, with momentum being a key factor[5].

The 2008 financial crisis acted as a significant milestone, emphasizing the need for adaptive momentum strategies. Post-crisis, as financial markets underwent substantial structural changes, the importance of algorithmic momentum trading surged. Algo traders began to combine traditional momentum strategies with emerging fields like machine learning and [artificial intelligence](/wiki/ai-artificial-intelligence), setting the stage for the current landscape of momentum algo trading.

## Fundamentals of Momentum in Algorithmic Trading

At its core, the mechanism behind momentum strategies in [algorithmic trading](/wiki/algorithmic-trading) lies in a two-step process:

1. **Identification**: Algorithms first identify momentum by analyzing historical data, considering factors like volume and volatility. They typically employ statistical measures, such as moving averages or rate of change, to spot trends. When the current price moves above the average price of a certain period, it's an indicator of positive momentum, while a move below suggests negative momentum.
2. **Execution**: Once momentum is identified, algorithms execute trades based on predetermined rules. For instance, they might buy a security if its 50-day moving average surpasses the 200-day moving average, indicating a longer-term uptrend. These rules are not static; adaptive algorithms adjust their parameters in real-time based on incoming data, ensuring they remain optimized to current market conditions[6].

The importance of momentum strategies in algo trading is underscored by the efficiency and speed they offer. While human traders might recognize and act on momentum-based strategies over hours or days, algorithms can detect and act on these opportunities within milliseconds. This rapid response time becomes especially valuable in volatile markets where price trends can change rapidly.

Moreover, momentum strategies have historically provided strong returns compared to other trading strategies, making them attractive for both institutional and retail traders[7]. By utilizing algorithms, traders can quickly scale their strategies, applying them to multiple securities or markets simultaneously. This scalability, coupled with the potential for high returns, drives the widespread adoption of momentum strategies in algorithmic trading.

## A Deeper Dive into Technical Indicators

Technical indicators serve as statistical measures that traders use to forecast market trends, providing a pathway for translating price information into actionable, quantifiable insight. Moving Averages (MA) and Relative Strength Index (RSI) stand prominently amongst the array of tools utilized to discern momentum in financial markets.

**Moving Averages**, primarily Simple Moving Average (SMA) and Exponential Moving Average (EMA), quantify average prices over a defined period, ironing out price fluctuations to offer a smoother trend line[8]. SMA calculates the arithmetic mean of prices over a set duration, while EMA gives greater weight to recent prices, making it more sensitive to new trends. Traders leverage crossovers, where short-term MAs cross above or below long-term MAs, as signals for potential momentum shifts. For instance, the "Golden Cross" - where the 50-day MA moves above the 200-day MA - is frequently heralded as a bullish momentum signal[9].

The **Relative Strength Index**, on the other hand, quantifies momentum by measuring the speed and change of price movements, oscillating between zero and 100. Generally, an RSI above 70 indicates overbought conditions, suggesting the potential for a price decrease, while an RSI below 30 indicates oversold conditions, signaling a possible price increase[10]. Traders utilize these thresholds to pinpoint moments where momentum may be escalating unsustainably, presenting an opportune moment to enter or [exit](/wiki/exit-strategy) trades.

In a practical application, the famous Turtle Trading strategy, developed by Richard Dennis and William Eckhardt, leveraged a form of Moving Average Crossover, where positions were taken or reversed based on 20-day and 55-day [breakout](/wiki/breakout-trading) levels[11]. This approach, founded upon momentum investing, underscores the practical use of moving averages to detect, and profit from, sustained price movements.

An illustrative case pertaining to RSI can be found in the periodic rallies of Bitcoin. Observing its weekly chart during the 2017 bull run reveals that each time Bitcoin's RSI crossed above 90, it was followed by a significant price correction[12]. Savvy traders, observing these momentum indicators, could act preemptively, either locking in profits or preparing for an entry point following the correction.

## Integrating Momentum Strategies with Machine Learning Algorithms

Harnessing the computational prowess of [machine learning](/wiki/machine-learning) (ML) can significantly augment momentum trading strategies, offering an innovative blend of technology and financial acumen.

The Decision Tree algorithm can create a model that predicts the target variable by learning decision rules from the features of the data. Within momentum trading, Decision Trees can be applied to decipher patterns from historical data, such as identifying specific technical indicator thresholds or price patterns that frequently precede a sizable price increase. By assessing the historical price and trading [volume](/wiki/volume-trading-strategy) data, Decision Trees can determine optimal entry and exit points for trades, furnishing traders with data-driven strategies to potentially augment returns[13].

ML algorithms, with their propensity for discerning patterns and adaptability, can minimize whipsaws (false signals) and dynamically adjust to varying market conditions. By leveraging ML, traders can develop more adaptive momentum trading strategies that refine themselves in alignment with evolving market dynamics, thereby ensuring their trading strategies remain robust and pertinent[14].

Deep learning, particularly Recurrent Neural Networks (RNNs), can further enhance momentum strategies. Unlike traditional algorithms, RNNs consider the sequence of data, making them suited for time-series forecasting prevalent in momentum trading. When applied to momentum strategies, RNNs facilitate the prediction of future prices by recognizing patterns and dependencies in historical price data, thereby proffering traders with insights driven not just by price and volume, but by discerning the latent patterns woven within them[15].

## Comprehensive Guide to Implementing Momentum Algo Trading

Embarking on the implementation of a momentum trading algorithm requires both strategic thinking and technical proficiency. Let's deep dive into the step-by-step process.

**Step 1**: **Data Acquisition and Processing**

Acquiring quality financial data is pivotal. Utilize APIs, like Alpha Vantage or Yahoo Finance, to retrieve historical price and trading volume data. You can also use [the Hugging Face datasets](https://huggingface.co/edarchimbaud). Ensure to clean and preprocess the data, handling any missing or outlier values.

```python
import pandas as pd
import yfinance as yf  # For more datasets, visit: https://paperswithbacktest.com/datasets

## Fetch historical data
data = yf.download('AAPL', start='2020-01-01', end='2023-01-01')

## Handle missing data
data = data.dropna()

## Calculate moving average
data['MA5'] = data['Close'].rolling(window=5).mean()
```

**Step 2**: **Indicator Calculation**

Compute momentum indicators, such as Moving Averages, to identify potential buy/sell signals.

```python
## Calculate 10-day momentum
data['Momentum'] = data['Close'] - data['Close'].shift(10)
```

**Step 3**: **Algorithm Formulation**

Design the algorithm, embedding the logic behind the momentum strategy. Use signals to determine entry and exit points.

```python
## Define a signal flag
data['Signal'] = 0  # Default to no signal
data['Signal'][data['Momentum'] > 0] = 1  # Buy signal
data['Signal'][data['Momentum'] <= 0] = -1  # Sell signal
```

**Step 4**: **Backtesting**

[Employ backtesting to validate the efficacy of the algorithm](https://blog.paperswithbacktest.com/p/how-to-collect-data-for-backtesting), adjusting parameters as necessary.

```python
## Define initial capital
initial_capital = float(100000.0)

## Create a DataFrame `positions`
positions = pd.DataFrame(index=data.index).fillna(0.0)

## Buy a 100 shares
positions['AAPL'] = 100*data['Signal']

## Initialize the portfolio with value owned
portfolio = positions.multiply(data['Close'], axis=0)

## Store the difference in shares owned
pos_diff = positions.diff()

## Add `holdings` to portfolio
portfolio['holdings'] = (positions.multiply(data['Close'], axis=0)).sum(axis=1)

## Add `cash` to portfolio
portfolio['cash'] = initial_capital - (pos_diff.multiply(data['Close'], axis=0)).sum(axis=1).cumsum()

## Add `total` to portfolio
portfolio['total'] = portfolio['cash'] + portfolio['holdings']

## Add `returns` to portfolio
portfolio['returns'] = portfolio['total'].pct_change()
```

**Step 5**: **Risk Management and Optimization**

Incorporate risk management tactics like setting stop-loss or take-profit levels. Optimize the strategy by iteratively tweaking parameters and retesting the algorithm.

Concurrently, several challenges may surface during implementation:

1. **Data Quality**: Ensure consistency and reliability of data, addressing discrepancies, and ensuring alignment with actual market figures.
2. **Overfitting**: Guard against over-optimizing your model to historical data, which may lead to misperformance in live trading.
3. **Computational Resources**: Efficiently managing computational resources to handle data processing, algorithm execution, and real-time trading without lag or delay.
4. **Regulatory and Compliance Issues**: Ensuring the algorithm abides by legal and trading platform restrictions and guidelines.
5. **Market Impact and Liquidity**: Consider the impacts of your trades on the market, especially if trading large volumes or in less liquid markets.

## Critical Analysis of Momentum Algo Trading

Momentum algo trading, despite its successes and popularity, is not immune to critiques and inherent risks. An understanding of these dimensions ensures a well-rounded perspective for any trader or developer.

**Risk Factors**:

1. **Market Volatility**: Momentum strategies, by their very nature, are contingent on trends in the market. Extreme market volatility can generate false signals, leading to potential losses. The 2008 financial crisis is a testament, where momentum strategies suffered due to sharp market reversals[16].
2. **Model Overfitting**: A frequently encountered risk in quantitative strategies is overfitting a model to historical data, leading it to perform poorly in live trading. This occurs when a model is too complex and captures noise instead of an underlying trend.
3. **Transaction Costs**: High-frequency trading based on momentum can lead to significant transaction costs. These costs can eat into potential profits, especially in strategies that require frequent rebalancing.
4. **Lack of Liquidity**: Engaging in momentum strategies in illiquid markets can result in significant price impacts, effectively eroding the profit potential of a trade.

**Drawbacks and Criticisms**:

1. **Short-Term Focus**: Critics often point out that momentum strategies, especially those in high-frequency trading, promote a short-term focus. This goes against the traditional investment philosophy of holding assets for long-term appreciation.
2. **Reversal Risks**: Momentum strategies are predicated on the continuation of trends. However, markets can and do reverse, leading to potential losses. The Dot-Com bubble's burst in the early 2000s is an example where momentum traders faced reversals[17].
3. **Crowding**: As momentum strategies have gained popularity, there's a risk of "crowding" where multiple traders act on similar signals, diluting potential profits.
4. **Economic Rationality**: Economists debate the very existence of momentum as a challenge to the Efficient Market Hypothesis (EMH). If markets are efficient, opportunities like momentum shouldn't persist. Critics argue that momentum profits might be compensation for bearing some unidentified systematic risk[18].

## Case Studies and Real-World Scenarios

One of the most notable success stories is that of the managed futures fund AQR Capital Management, which utilizes momentum as a significant part of its trading strategy[19]. Over the years, AQR has consistently employed sophisticated momentum models, leveraging both traditional price momentum and predictive signals from [alternative data](/wiki/best-alternative-data) sources. Their strategies, which seamlessly integrate momentum with other factors like value and quality, demonstrate how holistic approaches can produce more robust and consistent results in diverse market conditions.

Another shining example comes from the world of commodities trading. In 2008, during the unprecedented surge in oil prices, many momentum-based strategies, including those by prominent commodity trading advisors ([CTA](/wiki/cta-strategy)s), yielded stellar returns. These strategies capitalized on the strong uptrend in [crude oil](/wiki/crude-oil) prices, demonstrating the effectiveness of momentum models in trending markets.

However, success is not always guaranteed. In contrast to the aforementioned successes, there were also instances when momentum-based strategies faced challenges. For example, during the financial crisis of 2008, while some momentum strategies profited from the downward spiral of equities, others that were overly reliant on historical data without adaptive mechanisms faced significant drawdowns. This scenario underscored the vulnerability of static models that don’t adjust to shifting market regimes[20].

Such episodes emphasize a crucial lesson: while momentum can be a powerful factor in driving returns, it must be approached with caution. Over-reliance without proper diversification, adaptive measures, or risk management techniques can lead to significant losses.

## Future Perspectives

A notable trend in the financial technology sector has been the increasing integration of Artificial Intelligence (AI) into trading algorithms. For instance, Machine Learning (ML) models, particularly [deep learning](/wiki/deep-learning) and [neural network](/wiki/neural-network)s, are utilized to analyze market momentum by identifying patterns and trends in [vast datasets](https://paperswithbacktest.com/datasets) beyond human capability. These technologies enable algorithms to adapt to changing market conditions autonomously, enhancing the robustness of momentum strategies.

Blockchain, hailed as a disruptive technology, is poised to potentially alter the landscape of trading. With the adoption of Decentralized Finance (DeFi), blockchain could redefine how assets are traded and owned, offering opportunities for new types of momentum strategies based on decentralized assets and platforms. Decentralized exchanges (DEXs) and automated market makers (AMMs), for instance, provide novel environments where momentum trading algorithms might be applied or need to be adapted to account for the unique market mechanics.

Meanwhile, alternative data is gaining prominence, opening avenues for the development of momentum strategies that consider non-traditional data sources, such as social media sentiment, satellite imagery, and internet of things (IoT) data, to make informed trading decisions. Employing this alternative data, algo traders might develop more sophisticated momentum strategies that capitalize on insights gleaned from diverse and unconventional data streams.

## Strategies for Beginners to Advanced Traders

Here, we walk through a spectrum of strategies suitable for both novices and experts.

**For the Novices**:

1. **Start Simple**: Before delving deep into complex algorithms, familiarize yourself with basic momentum indicators like moving averages (MA) and the Relative Strength Index (RSI). These indicators, when combined, can offer a straightforward picture of a stock's momentum. For instance, an asset price moving above its 50-day MA might be considered bullish[8].
2. **Paper Trading**: Before committing real capital, use simulated trading platforms to test out your strategies. This risk-free environment allows you to understand how momentum factors play out without any financial repercussions.
3. **Stay Educated**: The world of trading is ever-evolving. Dedicate time each week to learn more about momentum strategies, be it through online courses, books, or webinars.
4. **Risk Management**: Set aside a fixed portion of your capital for momentum algo trading. It's also essential to set stop-loss levels to mitigate significant losses in volatile markets.

**For the Seasoned Traders**:

1. **Diversify Across Timeframes**: While many traders might focus on daily or weekly momentum, exploring intraday momentum can provide additional trading opportunities and diversification[21].
2. **Combine Momentum with Other Factors**: Incorporating additional factors like value, size, or volatility can provide a more holistic trading strategy. For instance, stocks that display strong momentum and are undervalued might offer better long-term returns.
3. **Backtesting with Out-of-Sample Data**: Ensure that your algorithms are not just curve-fitted to past data. [Regularly backtest your strategies using out-of-sample data](https://blog.paperswithbacktest.com/p/how-to-collect-data-for-backtesting) to ensure robustness[22].
4. **Machine Learning Enhancements**: With the advent of AI, traditional momentum strategies can be improved. Techniques like neural networks can help in identifying nonlinear patterns in momentum that might be elusive to traditional algorithms.
5. **Stay Updated with Market Dynamics**: Markets change, and what worked a decade ago might not work today. Regularly review, refine, and if necessary, overhaul your strategies to stay aligned with current market conditions.
6. **Collaboration and Networking**: Join forums, attend conferences, and actively engage with other traders. Often, shared experiences can provide insights into potential refinements or entirely new strategies.

## Conclusion

Momentum in algorithmic trading involves using statistical patterns, financial theories, and tech advancements to strategically capitalize on market trends and potentially generate profits. It goes beyond the basic principle of buying high and selling higher, integrating technical indicators and machine-learning algorithms to identify and leverage market trends. Moving Averages and the Relative Strength Index are key indicators for identifying potential trading moments, while machine-learning models like K Nearest Neighbour and Decision Trees enhance the precision of trading signals.

The application of these momentum strategies, illustrated through various case studies, highlights both potential outcomes and associated risks. Evolving technologies like AI and Blockchain are pivotal, shaping the future of momentum algorithmic trading. Navigating this constantly shifting landscape requires keeping pace with emerging trends, technological advancements, and global implications, while also adhering to ethical and legal standards across varying global markets and regulatory contexts.

Your insights and experiences as traders or enthusiasts play a crucial role in this ongoing dialogue in algorithmic trading. We encourage you to share your thoughts and experiences to further enrich this discussion. May your trades harness the momentum effectively!

## References & Further Reading

[1]: Jegadeesh, Narasimhan, and Sheridan Titman. ["Returns to Buying Winners and Selling Losers: Implications for Stock Market Efficiency."](https://www.jstor.org/stable/2328882) The Journal of Finance, vol. 48, no. 1, 1993, pp. 65-91.

[2]: Hong, Harrison, and Jeremy C. Stein. ["Differences of Opinion, Short-Sales Constraints, and Market Crashes."](https://www.jstor.org/stable/1262683) Review of Financial Studies, vol. 16, no. 2, 2003, pp. 487-525.

[3]: Cowles, Alfred. ["Can Stock Market Forecasters Forecast?"](https://www.jstor.org/stable/1907042) Econometrica: Journal of the Econometric Society, 1933, pp. 309-324.

[4]: Lefèvre, Edwin. ["Reminiscences of a Stock Operator."](https://www.amazon.com/Reminiscences-Stock-Operator-Edwin-Lef%C3%A8vre/dp/0471770884) John Wiley & Sons, 1923.

[5]: Asness, Cliff S., et al. ["Fact, Fiction, and Momentum Investing."](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2435323) Journal of Portfolio Management, vol. 40, no. 5, 2014, pp. 75-92.

[6]: Chan, L. K. C., and Lakonishok, J. ["Momentum Strategies."](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=225438) The Journal of Finance, vol. 51, no. 5, 1996, pp. 1681-1713.

[7]: Carhart, M. M. ["On Persistence in Mutual Fund Performance."](https://www.jstor.org/stable/2329556) The Journal of Finance, vol. 52, no. 1, 1997, pp. 57-82.

[8]: Murphy, J. J. ["Technical Analysis of the Financial Markets: A Comprehensive Guide to Trading Methods and Applications."](https://www.amazon.com/Technical-Analysis-Financial-Markets-Comprehensive/dp/0735200661) New York Institute of Finance, 1999.

[9]: Appel, G. ["The Moving Average Convergence Divergence Trading Method."](https://books.google.fr/books/about/The_Moving_Average_Convergence_divergenc.html?id=8DUxtAEACAAJ&redir_esc=y) Traders Press, 1985.

[10]: Wilder Jr, J. W. ["New Concepts in Technical Trading Systems."](https://www.amazon.com/New-Concepts-Technical-Trading-Systems/dp/0894590278) Trend Research, 1978.

[11]: Faith, C. ["Way of the Turtle: The Secret Methods that Turned Ordinary People into Legendary Traders."](https://www.amazon.com/Way-Turtle-Methods-Ordinary-Legendary/dp/007148664X) McGraw Hill Professional, 2007.

[12]: "Bitcoin Price Charts." CoinDesk, [https://www.coindesk.com/price/bitcoin](https://www.coindesk.com/price/bitcoin). Accessed 2023.

[13]: Dash, M., et al. ["Feature selection for clustering - A filter solution."](https://ieeexplore.ieee.org/document/1183893) Proceedings of the second international workshop on Clustering high dimensional data and its applications. 2002.

[14]: Prado, Marcos Lopez de. ["Advances in Financial Machine Learning."](https://www.amazon.com/Advances-Financial-Machine-Learning-Marcos/dp/1119482089) Wiley, 2018.

[15]: Bao, W., Yue, J., & Rao, Y. ["A deep learning framework for financial time series using stacked autoencoders and long-short term memory."](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0180944) PloS one, 12(7), e0180944. 2017.

[16]: Jegadeesh, N., & Titman, S. (2001). [“Profitability of Momentum Strategies: An Evaluation of Alternative Explanations”](https://www.jstor.org/stable/222579). The Journal of Finance, 56(2), 699-720.

[17]: Chabot, B., Ghysels, E., & Jagannathan, R. (2019). [“Momentum Trading, Return Chasing, and Predictable Crashes”](https://www.nber.org/system/files/working_papers/w20660/w20660.pdf). The Review of Financial Studies, 32(11), 4402-4442.

[18]: Fama, E. F., & French, K. R. (1996). [“Multifactor Explanations of Asset Pricing Anomalies”](https://onlinelibrary.wiley.com/doi/10.1111/j.1540-6261.1996.tb05202.x). The Journal of Finance, 51(1), 55-84.

[19]: Asness, C. S., Moskowitz, T. J., & Pedersen, L. H. (2013). [“Value and momentum everywhere“](https://pages.stern.nyu.edu/~lpederse/papers/ValMomEverywhere.pdf). The Journal of Finance, 68(3), 929-985.

[20]: Daniel, K., & Moskowitz, T. J. (2016). [“Momentum crashes“](https://www.sciencedirect.com/science/article/pii/S0304405X16301490). Journal of Financial Economics, 122(2), 221-247.

[21]: Chong, T. T. L., & Ip, W. H. (2009). [“Do momentum-based strategies still work in foreign currency markets?”](https://www.jstor.org/stable/4126758). Journal of Financial and Quantitative Analysis, 44(2), 253-273.

[22]: Bailey, D. H., & Lopez de Prado, M. (2018). [“The Deflated Sharpe Ratio: Correcting for Selection Bias, Backtest Overfitting, and Non-Normality”](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2460551). Journal of Portfolio Management, 40(5), 94-107.