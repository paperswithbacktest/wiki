---
title: "Turtle Trading and Algo Trading"
description: Turtle Trading, pioneered by Richard Dennis and William Eckhardt in the 1980s, revolutionized trend-following strategies by teaching a select group of novices systematic trading rules that focused on breakout signals, risk management, and disciplined position sizing. This article explores the core principles of Turtle Trading, its evolution in modern markets, and how it remains relevant in today's algorithmic trading landscape. Learn how to implement Turtle Trading strategies with tools like Python, risk management techniques, and insights from industry leaders.
---

![Trend-following-backtest-1024x726.png](images/Trend-following-backtest-1024x726.png)

## Table of Contents

## What is the Turtle Trading Strategy?

The Turtle Trading Strategy is a trend-following trading system developed in the 1980s by legendary traders Richard Dennis and William Eckhardt. It emerged from an experiment to settle a debate between the two about whether trading success could be taught or was an innate skill. Dennis believed anyone could learn to trade profitably with a structured set of rules, while Eckhardt argued it required natural talent. To test this, they recruited a group of novices—nicknamed the "Turtles"—and trained them in a specific methodology.

At its core, the Turtle Trading Strategy is designed to capitalize on sustained market trends, whether upward or downward. It uses a mechanical, rules-based approach to remove emotion from trading decisions. The system relies heavily on technical indicators, particularly breakouts, where trades are entered when prices move beyond a defined range (like a 20-day or 55-day high or low). The Turtles were taught to buy when prices broke to new highs and sell when they hit new lows, betting that these breakouts signaled the start of a trend.

The strategy also incorporates strict risk management and position sizing rules to protect capital and maximize gains during big moves. It’s not about predicting the market but reacting to it systematically—letting winners run and cutting losers short. Originally applied to commodities like oil, gold, and currencies, its principles have since been adapted to stocks, forex, and other markets. While simple in concept, its success hinges on discipline and sticking to the rules, even during losing streaks.

## Who developed the Turtle Trading Strategy?

The Turtle Trading Strategy was developed by two prominent traders, Richard Dennis and William Eckhardt, in the early 1980s. Richard Dennis, often called the "Prince of the Pit," was a self-made millionaire known for turning a small initial investment into hundreds of millions through aggressive commodity trading. William Eckhardt, his longtime friend and collaborator, brought a more analytical perspective, with a background in mathematics and a methodical approach to markets.

![Untitled](images/Untitled%201.png)

The strategy’s origin stems from a bet between them. Dennis believed trading could be taught to anyone with the right system, while Eckhardt thought it required an inherent knack. To settle the dispute, they launched an experiment in 1983, recruiting a diverse group of beginners—later dubbed the "Turtles"—through a newspaper ad. Dennis and Eckhardt trained these novices in their trend-following system, proving Dennis’s point when many of the Turtles went on to earn substantial profits. Their partnership and this experiment birthed the Turtle Trading Strategy, blending Dennis’s bold intuition with Eckhardt’s disciplined framework.

## What is the main philosophy behind the Turtle Trading approach?

The main philosophy behind the Turtle Trading approach is that markets move in trends—sustained periods of upward or downward price movement—and that these trends can be systematically exploited for profit. It’s built on the idea that price action, not predictions or fundamentals, should drive trading decisions. The Turtles were taught to "trade what they see," reacting to breakouts and momentum rather than guessing where the market might go next.

This philosophy hinges on a few key beliefs. First, trends are rare but powerful, so you have to catch the big moves to offset smaller, frequent losses. Second, human emotions like fear and greed derail success, so a rigid, mechanical set of rules is essential to enforce discipline. Third, trading is a numbers game—consistency and probability matter more than being right every time. The Turtles didn’t aim to outsmart the market; they aimed to ride its waves, letting winners run while ruthlessly cutting losers. It’s a patient, reactive approach that prioritizes sticking to the system over intuition or ego.

## How does the Turtle Trading Strategy use trend-following principles?

The Turtle Trading Strategy uses trend-following principles by focusing on capturing sustained price movements in markets, betting that once a trend starts, it’s likely to continue. It’s all about identifying and riding these waves rather than predicting reversals. The Turtles relied on technical signals—specifically breakout points—to spot when a trend might be kicking off. For example, they’d buy when a price broke above a 20-day or 55-day high, signaling potential upward momentum, or sell short when it dropped below a similar low.

The strategy doesn’t care why the trend is happening—economic news, supply shifts, or market psychology—it just reacts to the price action. Once in a trade, the Turtles let it run as long as the trend held, using trailing stops to lock in profits without jumping out too early. They also accepted that most trades might fail, but the few big winners would more than make up for it. This methodical, hands-off approach ensures they stay aligned with the market’s direction, leveraging momentum while avoiding overthinking or second-guessing. It’s trend-following distilled to its essence: ride the move, cut the noise.

## What are the key rules for entering a trade in the Turtle system?

The core principles of Turtle Trading form a methodology that’s both strict and systematic, aimed at capturing trends based on predefined signals while managing risk meticulously. Richard Dennis, the architect of the Turtle Trading strategy, built it around a framework of rules that were simple to follow but disciplined in nature.

![Untitled](images/Untitled.png)

**Original Rules Breakdown**

The original Turtle Trading rules revolve around a concept called '[breakout](/wiki/breakout-trading) trading', which signifies entering the market when prices move beyond a certain threshold. The Turtles would enter a long position (buy) when the price exceeded the high of the previous 20 days or take a short position (sell) when it dropped below the low of the last 20 days. Mathematically, this can be represented as:

- Entry Long: If Price today > High of the Last 20 Days, then Buy.
- Entry Short: If Price today < Low of the Last 20 Days, then Sell.

These simple price channels, known as Donchian Channels, are pivotal to the Turtle methodology and can be expressed using the formula:

$\text{Donchian Channel} = \text{Max/Min}(\text{High/Low over last N periods})$

**Position Sizing and Risk Management**

Central to the Turtles' success was rigorous risk management, particularly their rule on position sizing. The Turtles used the Average True Range (ATR), a measure of market volatility, to determine the size of their trading units. A single unit would be the amount they could trade based on a 1% ATR of the market price. For a given market with price $P$ and ATR $A$, a unit size $U$ could be calculated as:

$U = \frac{Account Equity \times Risk Percentage}{A \times Dollar Volatility}$

Where $DollarVolatility = P \times A$, and Risk Percentage typically 1% or 2% of account equity.

**Entry and Exit Strategies**

After entering a position, the Turtles implemented a pyramiding strategy, adding to the trade in increments of 1/2 N as the price moved in their favor, not to exceed four units total to prevent overexposure.

For [exit](/wiki/exit-strategy) strategies, the Turtles set stop losses at 2 N below the entry for long positions and above the entry for short positions. They would also exit positions when the price broke a 10-day high or low, depending on whether they were short or long, in essence reversing their breakout entry signal.

**Trend Following Methodologies**

The crux of the Turtle system was a trend-following strategy that capitalizes on large and sustained price movements. The idea was not to predict or anticipate trends but to respond to them with the assurance that many small losses could be outweighed by large and infrequent gains on major trends.

**Psychological Discipline**

An often-underestimated aspect of the Turtle Trading system is the psychological discipline required to follow the rules without deviation. Dennis stressed the importance of following the system with an almost stoic calm, ignoring the emotional swings that financial markets can induce.

Psychological resilience was quantified in terms of sticking to the defined risk parameters and not deviating from the system due to market noise or personal beliefs about where the market is heading. This can be summarized by the Turtles' mantra:

> "Follow the rules, follow the system. Success is a function of your discipline."
> — Richard Dennis

## How do the Turtles determine position sizing?

**Volatility-Based Position Sizing**

Position sizing was central to the Turtles' risk management strategy, determined by market volatility. Using the Average True Range (ATR), a metric that captures the degree of price volatility, the Turtles would adjust the size of their trade. The idea was to normalize the volatility of different markets, allowing for consistent risk management across trades. The position size $P$ was defined as:

$P = \frac{N \times Account Equity}{ATR}$

Here, $N$ is the risk [factor](/wiki/factor-investing) decided by the trader, often 1% of the account equity, ensuring no single trade could incur a loss greater than the predetermined risk threshold.

**Pyramiding Strategies**

The Turtles employed a pyramiding strategy, adding to their positions as the market moved in their favor, but only up to a maximum of four units to avoid overexposure. Each additional unit could be added for every $\frac{1}{2} ATR$ price move in the profitable direction, creating an opportunity for compounded growth while maintaining risk control.

## What are the exit strategies in Turtle Trading?

**Stop-Loss Techniques**

Stop-loss orders were integral to the Turtle strategy, placed at 2 ATRs away from the entry price. This allowed the Turtles to limit their losses on any given trade while providing enough market "breathing room." The calculation for a stop-loss level $S$ on a long position entered at price $E$ is:

$S = E - (2 \times ATR)$

This strategy aimed to prevent the emotion-driven decisions that often lead to larger losses or the cutting of profitable trades too early.

**Profit-Taking Methods and Exit Rules**

Profit-taking for the Turtles was as systematic as their entry strategy. They would exit trades when the price action moved against the trend by a certain amount, typically the 10 or 20-day low for long positions and the 10 or 20-day high for short positions, effectively reversing their breakout strategy for exits.

## How does risk management work in the Turtle Trading Strategy?

![Untitled](images/Untitled%202.png)

Risk management in the Turtle Trading Strategy is a cornerstone of its design, built to protect capital while maximizing gains from big trends. It’s systematic and precise, relying on rules rather than gut feel. The Turtles used a concept called "N"—a measure of a market’s volatility, calculated as the 20-day average true range (ATR)—to gauge how much risk to take. This kept their bets proportional to how much a market typically moved, avoiding overexposure in choppy conditions.

Position sizing was tied to this. They risked a fixed percentage of their account—usually 1% or 2%—per trade. Using N, they’d figure out how many contracts or shares they could buy so that a 1N move against them wouldn’t exceed that risk limit. For example, if N was $1 and their account allowed a $2,000 loss, they’d trade 2 units. This "volatility-adjusted" sizing meant smaller positions in wild markets and bigger ones in calmer ones.

They also diversified across uncorrelated markets—like oil, bonds, or currencies—to spread risk. Stops were non-negotiable: initial stops were set at 2N below the entry for longs (or above for shorts), ensuring quick exits on losers. As trends progressed, trailing stops moved with the price to lock in profits. The philosophy was simple: survive the small losses, stay in the game for the big wins. It’s a disciplined shield against the market’s chaos.

## What markets can the Turtle Trading Strategy be applied to?

![Trend-following-pnl-1024x658.png](images/Trend-following-pnl-1024x658.png)

The Turtle Trading Strategy can be applied to virtually any liquid market that exhibits trends, thanks to its focus on price action and adaptability. Originally, the Turtles traded commodities—think crude oil, gold, silver, coffee, sugar, and cotton—since those were the markets Richard Dennis and William Eckhardt thrived in during the 1980s. They also tackled futures contracts like currencies (e.g., Japanese yen, Swiss franc) and bonds (e.g., U.S. Treasuries), which offered the volatility and volume needed for trend-following.

Today, the strategy’s principles extend beyond its roots. You can use it in stocks, especially large-cap or index funds with clear momentum, though individual equities can be trickier due to less consistent trends. Forex markets, with pairs like EUR/USD or USD/JPY, are a natural fit given their liquidity and tendency to trend. Even newer arenas like cryptocurrencies—Bitcoin or Ethereum—work, as their wild swings often produce breakout opportunities.

The catch? It thrives best in markets with enough movement and depth. Illiquid or range-bound markets—like penny stocks or obscure assets—can choke it, since the strategy needs trends to breathe. As long as there’s price data and a pulse, the Turtle system can theoretically strap in and ride.

## What are the advantages and disadvantages of Turtle Trading?

The Turtle Trading Strategy comes with clear strengths and weaknesses, shaped by its mechanical, trend-following nature.

### Advantages
1. **Simplicity**: The rules are straightforward—buy breakouts, set stops, size positions by volatility. No complex analysis or insider knowledge needed.
2. **Big Wins**: It’s built to catch massive trends, so when markets move hard (like commodity booms or currency runs), profits can be outsized.
3. **Discipline**: By removing emotion, it forces consistency, which is gold for traders who struggle with second-guessing or panic-selling.
4. **Adaptability**: It works across markets—stocks, forex, futures, crypto—as long as there’s liquidity and momentum.
5. **Risk Control**: Built-in position sizing and stops limit losses, keeping you in the game even through rough patches.

### Disadvantages
1. **Frequent Losses**: Most trades fail because trends are rare. You endure a lot of small cuts waiting for the big payoff, which tests patience.
2. **Whipsaws**: In choppy, sideways markets, breakouts often fake out, racking up losses with no trend to ride.
3. **Lag**: It’s reactive, not predictive. You’re late to the party on trends and might exit after the peak, missing some gains.
4. **Emotional Grind**: Sticking to the system during a losing streak—or watching profits erode before an exit—can be brutal, even if it’s “mechanical.”
5. **Capital Hunger**: To handle volatility-based sizing and diversification, you need a decent account size. Small traders might find it tough to scale.

It’s a trade-off: you get a shot at home runs, but you’ve got to stomach a lot of strikeouts. Works best if you’ve got the grit and the bankroll to let it play out.

## How can a beginner start implementing the Turtle Trading Strategy?

A beginner can start implementing the Turtle Trading Strategy by breaking it down into manageable steps, keeping it simple while building confidence. Here’s how to get rolling:

First, **learn the basics**. Understand the core idea: you’re buying breakouts (like a 20-day high) and selling short on breakdowns (like a 20-day low) to catch trends. Grab a free charting tool—think TradingView or a broker’s platform—and pick a market with decent movement, like a major forex pair (EUR/USD) or an ETF (SPY). No need to overcomplicate it with obscure stuff early on.

Next, **set up your rules**. Use the original Turtle framework as a guide: enter a trade when the price breaks a 20-day high/low, place a stop-loss at 2 times the 20-day average true range (ATR) below/above your entry, and exit on a 10-day low/high for longs/shorts. You can test this manually or with a demo account. For position sizing, keep it tiny—risk just 1% of a small practice account (say, $10 on a $1,000 balance) per trade, using ATR to scale your position.

Then, **practice with paper trading**. Pick one or two markets, track daily prices, and log every trade—entry, stop, exit, profit/loss. Don’t skip this; it builds discipline without torching real money. Spend a month or two seeing how it feels when trades flop (they will) and trends hit (they might).

Finally, **start small with real cash**. Once you’re comfortable, fund a modest account—$500 or $1,000 works—and trade micro-lots or fractional shares. Stick to the rules religiously, even when it sucks. Use a spreadsheet to track results and tweak only after you’ve got solid data.

Setting up a Turtle Trading strategy in Python requires a systematic approach to coding the rules laid out by Richard Dennis and William Eckhardt. Here's a streamlined guide to help you begin coding your Turtle Trading strategy:

1. **Install Python:** Ensure you have Python installed on your machine. If not, download and install it from the official Python website.
2. **Set Up Your Development Environment:** You can use an IDE like PyCharm or a more interactive environment like Jupyter Notebook, which is great for data analysis.
3. **Import Necessary Libraries:** You’ll need pandas for data manipulation, NumPy for numerical calculations, and matplotlib for plotting graphs. You can import these libraries using the following code:
    
    ```python
    import pandas as pd
    import numpy as np
    import matplotlib.pyplot as plt
    ```
    
4. **Get Historical Data:** Fetch historical price data for the asset you wish to trade. You can use libraries like `yfinance` to download data directly into Python:
    
    ```python
    import yfinance as yf  # For more datasets, visit: https://paperswithbacktest.com/datasets
    data = yf.download('AAPL', start='2010-01-01', end='2023-01-01')
    ```
    
5. **Implement the Donchian Channel:** This is used to determine buy and sell signals. Calculate the upper and lower bounds with a 20-day window for entry signals and a 10-day window for exit signals:
    
    ```python
    data['20_day_high'] = data['Close'].rolling(window=20).max()
    data['10_day_low'] = data['Close'].rolling(window=10).min()
    ```
    
6. **Position Sizing:** According to Turtle rules, position sizing is based on the market's volatility. Calculate the Average True Range (ATR) to assess volatility:
    
    ```python
    data['ATR'] = data['Close'].rolling(window=20).apply(lambda x: np.max(x) - np.min(x))
    ```
    
7. **Entry Signals:** Generate entry signals based on a breakout from the Donchian Channel. If today's price is greater than the 20-day high, it's a buy signal:
    
    ```python
    data['Buy_Signal'] = np.where(data['Close'] > data['20_day_high'].shift(1), 1, 0)
    ```
    
8. **Exit Signals:** Similarly, generate exit signals. If today's price is lower than the 10-day low, it's a sell signal:
    
    ```python
    data['Sell_Signal'] = np.where(data['Close'] < data['10_day_low'].shift(1), -1, 0)
    ```
    
9. **Risk Management:** Implement a stop-loss as a risk management tool. This could be a fixed percentage from the entry price or a multiple of ATR:
    
    ```python
    data['Stop_Loss'] = data['Buy_Signal'] * (data['Close'] - 2 * data['ATR'])
    ```
    
10. **Backtesting:** Simulate the trading strategy on historical data to see how it would have performed. Track the equity curve, drawdowns, and other performance metrics.
11. **Optimize:** Fine-tune the parameters, such as the look-back periods for the Donchian Channel or the risk per trade, based on the backtesting results.
12. **Plot Results:** Use matplotlib to visualize entry and exit points, alongside your asset’s price action over time.
13. **Live Testing:** Consider running your algorithm in a paper trading environment before going live to ensure it behaves as expected.

<aside>
👉 Tips on maintaining discipline and consistency:

- **Automate as Much as Possible:** The fewer manual steps, the less room there is for emotional decision-making.
- **Keep a Trading Journal:** Document all trades, including the reason for entry and exit and the emotional state at the time.
- **Regular Review:** Set aside time weekly or monthly to review the performance and adherence to the strategy.
- **Adherence to Risk Management Rules:** Never compromise on risk management rules. They are the lifeline of your trading career.
- **Continuous Learning:** Stay up to date with market conditions as they can affect the performance of your turtle trading strategy.
</aside>

Remember, while backtesting can provide insights into how a strategy might perform, it is not a guarantee of future results. Markets evolve, and strategies need to be adaptable. Always ensure that any trading strategy is well-tested and that you're prepared for the possibility of loss as well as gain.

## What advanced techniques can experienced traders use to optimize Turtle Trading?

Experienced traders can optimize the Turtle Trading Strategy by fine-tuning its mechanics and adapting it to modern markets while staying true to its trend-following roots. Here are some advanced techniques to level it up:

1. **Filter Breakouts**: Add confirmation tools to reduce whipsaws. For instance, pair the 20-day or 55-day breakout with a momentum indicator like the ADX (Average Directional Index)—only take trades when ADX shows a strong trend (e.g., above 25). This cuts noise in choppy markets.

2. **Dynamic Timeframes**: Adjust the breakout periods based on market conditions. Instead of a fixed 20-day or 55-day high/low, test a shorter 10-day entry for fast-moving markets (like crypto) or a longer 100-day for slower ones (like bonds). Backtest to find the sweet spot.

3. **Volatility Scaling**: Refine position sizing beyond the basic 1% risk per N (ATR). Scale up slightly in low-volatility periods to capture more of a move, or down in high-volatility spikes to dodge blowups. Use a volatility index (like VIX for stocks) as a guide.

4. **Portfolio Rotation**: Diversify smarter by rotating into trending markets. Scan a basket of assets weekly—stocks, forex, commodities—and weight trades toward those with the strongest momentum (e.g., highest 50-day returns). This keeps capital chasing the best opportunities.

5. **Trailing Stop Tweaks**: Upgrade the exit strategy. Instead of a fixed 10-day low/high, experiment with a Chandelier Exit (ATR-based trailing stop) or a percentage-based trail (e.g., lock in gains after a 20% move). This can squeeze more profit from runaway trends.

6. **Pyramiding**: Add to winning positions as the trend strengthens, a Turtle staple. But optimize it—stack smaller incremental units (e.g., half the initial size) at wider intervals (like every 2N move) to balance reward and risk.

7. **Machine Learning Edge**: Use data-driven tools to spot patterns. Train a simple model to predict breakout success based on historical price action, volume, or seasonality. It’s not about overriding the system but flagging higher-probability setups.

8. **Time-Based Exits**: Cap trade duration to avoid stagnation. If a position hasn’t moved significantly in 30 days, exit and redeploy capital elsewhere. This keeps your money active in a trendless grind.

Backtesting is non-negotiable—run these tweaks through historical data (or a platform like MetaTrader) to quantify edge before going live. The catch: over-optimization can kill the system’s simplicity, so keep changes incremental and stress-test them in real-time with small positions. The goal is to sharpen the blade, not reinvent it—stay disciplined, and let the trends do the heavy lifting.

Quantitative turtle trading strategies introduce a new dimension to the classic Turtle Trading system, incorporating data analysis and computational algorithms to identify trends and generate signals. These strategies use historical data and statistical methods to optimize the trading rules and parameters, such as entry/exit points and position sizing. The quantitative approach can also integrate machine learning models to adapt to changing market conditions, attempting to improve upon the profitability and robustness of the traditional trend-following systems.

Research in quantitative finance, such as papers published in the "Journal of Portfolio Management," suggests that applying machine learning techniques can enhance the performance of trend-following strategies. Quantitative models can digest a vast array of market data at high speed, enabling traders to capture trends that may not be immediately apparent to the human eye.

Moreover, advancements in computing power and the proliferation of open-source programming languages, like Python, have democratized the implementation of quantitative strategies. Tools such as pandas for data analysis, NumPy for numerical computation, and scikit-learn for machine learning have become staples in the quant trader's toolkit. These technologies facilitate the development of complex trading models that can process large datasets to identify potentially profitable trends and patterns in market prices.


## References & Further Reading

[1]: Covel, Michael W. ["The Complete TurtleTrader: How 23 Novice Investors Became Overnight Millionaires."](https://en.wikipedia.org/wiki/The_Complete_TurtleTrader) HarperCollins, 2009

[2]: Russell Sands' ["The Original Turtle Trading Rules"](https://www.amazon.com/Original-Turtle-Trading-Rules/dp/1592803466)

[3]: Michael Covel's ["Trend Following"](https://www.trendfollowing.com/)

[4]: ["Following the Trend"](https://www.followingthetrend.com/) by Andreas Clenow

[5]: ["Way of the Turtle"](https://www.goodreads.com/book/show/503534.Way_of_the_Turtle) by Curtis Faith

[6]: [Turtle Trading Experiement A Successful Market Legend](https://www.investopedia.com/articles/trading/08/turtle-trading.asp)

[7]: [Turtle trading rules Does it still work today](https://www.tradingwithrayner.com/turtle-trading-rules/)

[8]: [Turtle Trading System Rules and Strategy](https://fxopen.com/blog/en/turtle-trading-system-rules-and-strategy/)

[9]: [What is Turtle Trading Turtle Trading Rules](https://www.ig.com/en/trading-strategies/turtle-trading--what-is-it-and-what-are-the-rules--180904)

[10]: [Original Turtle Trading Rules Philosophy](https://www.turtletrader.com/rules/)