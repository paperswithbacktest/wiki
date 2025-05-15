---
title: "3 Bullish Candlestick Patterns That Work (Algo Trading)"
description: Explore algorithmic trading through the lens of bullish candlestick patterns, essential tools for predicting upward market trends. This guide investigates into integrating patterns like Hammer, Bullish Engulfing, and Morning Star into trading systems, enhancing strategy and execution. Discover backtesting insights and how automated recognition of these patterns can optimize trading efficiency by reducing human error and capitalizing on high-frequency opportunities. Whether you're refining current systems or starting anew, this resource offers valuable perspectives on leveraging bullish patterns for improved profitability.
---

![Image](images/1.png)

## Table of Contents

Candlestick chart patterns are a staple of technical analysis, used to infer shifts in market sentiment from price action. Each pattern is formed by one or more candlesticks (price bars) and often signals which side – bulls or bears – is gaining control. In algorithmic trading, these visual patterns can be translated into strict mathematical rules, allowing trading bots to scan for bullish reversals and execute trades automatically. Popular bullish candlestick patterns include the **Bullish Engulfing**, **Hammer**, and **Morning Star**, among others. These patterns, when coded into an algorithmic strategy, serve as entry signals for long trades in anticipation of an upward trend reversal.

**Backtesting** such patterns is crucial to determine if they “work” – i.e. have predictive value – in real markets. Historically, many candlestick signals were accepted on faith, with **no empirical evidence** offered for their efficacy. Modern systematic trading flips this approach by using clear-cut definitions and running **algorithmic backtests**. Researchers have found that *some* candlestick patterns do exhibit quantifiable predictive value, especially when combined with trend filters. For example, certain bullish patterns show win rates well above 50% in data-driven tests. Still, these patterns are not foolproof – their reliability varies with context, and proper validation is needed to avoid false confidence.

In this article, we explore three bullish candlestick patterns commonly used in algorithmic trading systems. For each pattern, we provide a detailed definition, discuss the market psychology behind it, outline the price-action rules (with mathematical criteria), and demonstrate a Python implementation using the **Backtrader** backtesting framework. The code examples use historical daily data loaded via the `pwb-toolbox` (Papers With Backtest toolbox) repository, illustrating how to integrate pattern-detection strategies into an algo trading workflow. By the end, we will also discuss the backtesting results, reliability, and caveats of using these patterns in practice.

## Bullish Engulfing Pattern

The **Bullish Engulfing** is a classic two-candle reversal pattern that often marks the transition from a downtrend to an uptrend. It occurs when a **small bearish candle** (down day) is immediately followed by a **large bullish candle** (up day) that completely **engulfs** the prior candle’s body. In other words, the second candlestick’s real body covers the entire range of the first candlestick’s body. This pattern typically appears after a sustained down move, signaling that selling pressure may be exhausted and buyers are seizing control for a potential reversal upward.

### Pattern Definition and Psychology

In a downtrend, a bullish engulfing pattern reflects a dramatic shift in momentum. Day 1 (the smaller candle) is bearish, indicating the downtrend was still in force. Day 2 opens lower than Day 1’s close (often even lower than Day 1’s low) yet buyers step in aggressively, driving price up to close above Day 1’s open. This surge completely overtakes the previous day’s losses – **an “obvious win for the buyers”** as Investopedia describes it. The market psychology here is that the prior bearish sentiment has been overwhelmed by a sudden influx of bullish demand. Sellers who dominated on Day 1 are overrun by buyers on Day 2, suggesting the downtrend may have bottomed out. A bullish engulfing pattern is thus interpreted as a strong reversal signal: it **indicates that bears (sellers) have lost control and bulls (buyers) are taking over**.

**Identification rules:** To quantify a bullish engulfing pattern for algorithmic trading, we require:

* **Downtrend context:** The pattern should occur after a notable price decline (to increase the probability it’s a true reversal, not a continuation). For example, some traders require that the days leading up to it were predominantly bearish.
* **First candle:** A small **bearish** candlestick (Day 1) with a relatively short body. Its close is lower than its open (indicating a down day).
* **Second candle:** A larger **bullish** candlestick (Day 2) that opens below the previous day’s close and closes above the previous day’s open. The Day 2 candle’s real body completely overlaps (engulfs) Day 1’s body. In stricter definitions, the Day 2 range (high to low) might even exceed Day 1’s range, but the key criterion is that **Open<sub>2</sub>** and **Close<sub>2</sub>** straddle the entire body of Day 1.

Mathematically, if we denote Day 1’s open, high, low, close as *Open₁*, *High₁*, *Low₁*, *Close₁* and Day 2’s as *Open₂*, *High₂*, *Low₂*, *Close₂*, one can formalize the bullish engulfing conditions as:

$$
\begin{aligned}
&Close_1 < Open_1,  &(\text{Day 1 is bearish})\\ 
&Close_2 > Open_2,  &(\text{Day 2 is bullish})\\ 
&Open_2 \le Close_1, \\ 
&Close_2 \ge Open_1~. 
\end{aligned}
$$

The last two inequalities ensure Day 2’s body spans or exceeds Day 1’s body range. Essentially, Day 2’s open is at or below Day 1’s close, and Day 2’s close is at or above Day 1’s open. This encapsulates the engulfing aspect (even ignoring wicks). Traders often prefer the engulfing candle to be significantly larger (e.g. Day 2’s body length > Day 1’s body) to emphasize the force of the reversal. High trading volume on the second day can further confirm the pattern’s validity, indicating broad participation in the bullish reversal.

### Backtrader Implementation

Below is a Backtrader strategy that detects bullish engulfing patterns and enters long (buy) positions when they occur. We utilize daily stock data (in this example, **Apple Inc. (AAPL)**) retrieved via `pwb_toolbox.datasets`. The strategy checks each new bar for the engulfing criteria and executes a buy order at the next market open when a pattern is identified. For simplicity, no additional trend filter or exit logic is applied – the focus is solely on the entry signal from the candlestick pattern.

```python
# Bullish Engulfing Pattern Trading Strategy
import backtrader as bt
import pwb_toolbox.datasets as pwb_ds

class BullishEngulfingStrategy(bt.Strategy):
    def next(self):
        # Ensure we have at least 2 bars (yesterday and today) to evaluate
        if len(self.data) < 2:
            return
        # Get yesterday's and today's OHLC values
        prev_open, prev_close = self.data.open[-1], self.data.close[-1]
        prev_high, prev_low   = self.data.high[-1], self.data.low[-1]
        curr_open, curr_close = self.data.open[0],  self.data.close[0]
        # Check Bullish Engulfing conditions:
        if prev_close < prev_open and curr_close > curr_open:                       # day1 bearish, day2 bullish
            if curr_open <= prev_close and curr_close >= prev_open:                # day2 body engulfs day1 body
                self.buy()  # trigger a buy signal

# Load daily data for AAPL from pwb-toolbox
df = pwb_ds.load_dataset("Stocks-Daily-Price", ["AAPL"])
data = bt.feeds.PandasData(dataname=df)  # convert pandas DataFrame to Backtrader data feed

# Set up Backtrader engine
cerebro = bt.Cerebro()
cerebro.addstrategy(BullishEngulfingStrategy)
cerebro.adddata(data)
cerebro.run()
```

In this code, the strategy’s `next()` method compares the previous bar (`-1`) and the current bar (`0`) to identify the pattern. We explicitly check that the previous day was down (`prev_close < prev_open`) and the current day is up (`curr_close > curr_open`). The engulfing condition `curr_open <= prev_close and curr_close >= prev_open` ensures the current day’s body covers the prior day’s body range. When these conditions are met, `self.buy()` executes a market order (on the next bar’s open by default in Backtrader). In a complete strategy, one could add confirmation filters (e.g. requiring an overall downtrend, or waiting for a higher close the next day) and define an exit rule (such as selling after a few days or at a target profit). Here we illustrate the core entry signal generation.

## Hammer Pattern

The **Hammer** candlestick is a single-bar bullish reversal pattern characterized by its distinctive shape: it has a **small real body** near the top of the candle and a **long lower shadow** (wick) with little to no upper shadow. A hammer appears during a downtrend and signals that a price decline may be nearing its end, with an upward reversal potentially imminent. Visually, it looks like a “T” or hammer, where the handle (shadow) indicates that sellers pushed the price sharply lower intraday, only to have buyers step in and drive the price back up toward the open by the close. This bullish intraday reversal often presages a broader trend reversal to the upside.

### Pattern Definition and Psychology

For a candlestick to qualify as a hammer, it should meet these **criteria**:

* **Downtrend context:** The candle occurs after a series of declining prices (so that it represents a potential capitulation and reversal point). The effectiveness of the hammer is highest when it materializes at the tail end of a significant downtrend or near a known support level.
* **Small real body:** The real body (difference between open and close) is small and positioned near the candle’s high. The body can be either bullish (green/white) or bearish (red/black), though a bullish close is thought to signal a stronger reversal\*\*.\*\* The key is that the close is not far below the open, indicating price did not stay low.
* **Long lower shadow:** The lower wick should be **at least 2× the length of the body**. This long tail shows that the price dropped significantly during the session (reflecting intense selling), but then **buyers overpowered the sellers and pushed the price back up** before the close. Ideally, the lower shadow has no critical support below it, meaning it’s probing new lows that got rejected.
* **Minimal upper shadow:** There should be little or no wick above the body. A tiny upper shadow is acceptable (and common if the close is slightly below the high), but a very short top indicates that once buyers took the price up off the lows, the market was unable to sell back down much – consistent with bullish strength into the close.

In mathematical terms, let *Body* = |Close – Open|, *LowerShadow* = Open/Close (whichever is lower) – Low, and *UpperShadow* = High – Open/Close (whichever is higher). For a hammer pattern:

$$
LowerShadow \;\ge\; 2 \times Body, \qquad UpperShadow \;\approx\; 0~.
$$

Typically one might require *UpperShadow* to be no more than, say, 10% of the entire candle range, or even zero for an ideal hammer. For example, if a stock opened at \$100 and sold off to \$90 (intra-day low) but then rebounded to close at \$98, that day’s candle would have a long lower shadow ( \$8 length) and a small body (\$2 length). If the high was \$99, the upper shadow is \$1, which is very small. Such a candle fits the hammer profile: **lower shadow (8) ≥ 2 × body (2)**, and upper shadow (1) is negligible. This shape tells traders that although sellers drove prices to an extreme low, **buyers forcefully reversed the decline** and closed the session near the open, signaling a **potential shift from bearish to bullish momentum**. Essentially, the market “hammered out” a bottom, as the analogy goes.

Psychologically, the hammer represents a test of the market’s resolve in the downtrend. Early in the session, bears are fully in control (hence the sharp move down). But by the close, bulls have absorbed the selling and pushed the price back up – a clear indication that **demand is resurging** and the downtrend may be capitulating. Many traders view a hammer as one of the most reliable candlestick reversal signals, especially if confirmed by a subsequent bullish candle or other technical indicators (for instance, a bounce off a support line with increasing volume). Confirmation in the next session – such as a strong upward follow-through – is often sought to validate the hammer’s signal, because a single candle can sometimes give a false signal if not corroborated.

### Backtrader Implementation

Below we implement a strategy to detect hammer candles and buy when they occur. This strategy simply checks each day’s candle properties against the hammer criteria defined above. We again use `pwb_toolbox` to load historical daily data (using AAPL as an example). For brevity, we will not require a prior downtrend in code (though in practice one might include a filter that the 5-day or 10-day trend is down). We will also act immediately on the hammer without waiting for next-day confirmation in this basic strategy.

```python
# Hammer Candlestick Pattern Trading Strategy
import backtrader as bt
import pwb_toolbox.datasets as pwb_ds

class HammerStrategy(bt.Strategy):
    def next(self):
        if len(self.data) < 1:
            return
        # Calculate candle parts for the current bar
        open0   = self.data.open[0]
        close0  = self.data.close[0]
        high0   = self.data.high[0]
        low0    = self.data.low[0]
        body    = abs(close0 - open0)
        lower_wick = min(open0, close0) - low0    # distance from low to the lower of open/close
        upper_wick = high0 - max(open0, close0)   # distance from high to the higher of open/close
        # Hammer shape conditions
        if lower_wick >= 2 * body and upper_wick <= 0.1 * (high0 - low0):
            # Optional: ensure the candle is somewhat small compared to recent range or confirm trend
            # if needed, but here we directly signal a buy on any hammer-shaped candle.
            self.buy()

# Load daily data for AAPL
df = pwb_ds.load_dataset("Stocks-Daily-Price", ["AAPL"])
data = bt.feeds.PandasData(dataname=df)
# Set up and run the backtest
cerebro = bt.Cerebro()
cerebro.addstrategy(HammerStrategy)
cerebro.adddata(data)
cerebro.run()
```

In this code, we compute the candle’s body and wicks for each bar (`next()` processes one bar at a time). The strategy checks if the **lower\_wick** is at least twice the body and the **upper\_wick** is very small (here we enforce upper wick ≤ 10% of the total range as a proxy for “little or no” upper shadow). If these conditions are satisfied, `self.buy()` is called to initiate a long position. We do not explicitly check that the candle occurred after a prolonged downtrend in the code, but in practice one might add a condition like requiring the current close to be lower than the moving average or a certain percentage below recent highs, to ensure a downward context. Also, a real strategy might wait for confirmation – for example, buy if the next day’s price trades above the hammer’s high – rather than buying immediately at the close of the hammer day. Nonetheless, the above implementation captures the essence of algorithmically identifying a hammer candlestick pattern and acting on it.

## Morning Star Pattern

The **Morning Star** is a three-candle bullish reversal pattern that signals a transition from a bearish trend to a bullish trend. It is named “morning star” as it metaphorically represents the light of dawn (bullishness) emerging after a dark night (bearishness). This pattern consists of: (1) a long bearish candle, (2) a small-bodied candle that gaps down or at least closes below the first candle, and (3) a long bullish candle that closes well into the first candle’s body. When these three candles appear in sequence, they indicate that the downward momentum is waning and a reversal to the upside is likely underway. The morning star is considered a strong sign of *hope* and renewed buying pressure in what had been a gloomy downtrend.

### Pattern Definition and Psychology

A textbook **Morning Star** pattern unfolds as follows:

* **First candle:** A large **bearish** candlestick, extending the existing downtrend with a sharp price drop. This reflects continued intense selling – the “darkness before dawn.” It establishes the bearish mood, making it clear that sellers were in control up to that point.
* **Second candle:** A **small-bodied** candle (often a doji or a spinner) that opens lower than the first candle’s close (creating a gap down in markets where gaps occur). This candle can be either bearish or bullish, but the key is that it represents a **stall in the downtrend** – the selling pressure is subsiding. In an ideal morning star, this middle candle has **no overlap** with the body of the first candle (its entire range is below the first candle’s close), underscoring the gap in sentiment. The small body denotes indecision or equilibrium between buyers and sellers. Essentially, after the big drop on Day 1, Day 2’s market barely moved (or had a very narrow range), suggesting the prior bearish momentum is pausing.
* **Third candle:** A large **bullish** candlestick that opens higher than the second candle’s close and **closes deep into the first candle’s body**. Often, chartists look for the third candle’s close to be above the midpoint of the first candle’s body as a confirmation of a bullish reversal. This third day shows strong buying pressure returning to the market — it **“closes the gap”** and then some, erasing a good portion of the first candle’s decline. High volume on the third candle can strengthen confidence that this reversal signal is valid (indicating broad participation by bulls).

To formalize the **morning star** in an algorithmic way, let’s denote the three candles as Day 1, Day 2, Day 3. We require:

* Downtrend prior to Day 1 (subjective but can be defined by a series of lower lows, or a below-average price, etc.).
* Day 1: Large bearish candle (Close₁ << Open₁). For instance, one might require Day 1’s body to be longer than recent average candle length to ensure it’s a “big” down day.
* Day 2: Small real body (approximately a **doji** or small candle). A rough rule could be that Day 2’s body is a fraction of Day 1’s body (e.g., < 30% of Day 1’s length). Also, ideally **Low₂** and **High₂** are below **Close₁** (so that Day 2 is entirely below Day 1’s close, i.e., a gap in body if not in range). This gap criterion might be relaxed in continuous markets (like forex) where gaps are rare – the essence is that Day 2 remains at low price levels and does not retrace Day 1 significantly.
* Day 3: Large bullish candle (Close₃ >> Open₃). Critically, **Close₃ > (Open₁ + Close₁)/2**, meaning Day 3 closes **above the midpoint** of Day 1’s body. Strong forms of the pattern might even demand Close₃ almost up to Open₁ (recovering most of Day 1’s losses), but crossing the 50% mark of Day 1 is a common yardstick. Also, for a true morning star, **Open₃** is higher than **Close₂** (a gap up from the stagnant middle day), further reinforcing the shift in momentum.

As a formula, a simplified set of conditions could be:

$$
\begin{aligned}
&Close_1 < Open_1, \quad (\text{Day 1 bearish})\\ 
&|Close_2 - Open_2| << |Close_1 - Open_1|, \quad (\text{Day 2 small body})\\
&Close_3 > Open_3, \quad (\text{Day 3 bullish})\\ 
&Close_3 > \frac{Open_1 + Close_1}{2}~. \quad (\text{Close of Day 3 above Day 1's midpoint})
\end{aligned}
$$

The second line denotes that Day 2’s body is “much smaller” than Day 1’s (we use `<<` qualitatively here – one could set a specific ratio). The last condition is the critical confirmation of a bullish reversal: Day 3’s strong close well into Day 1’s losses.

The **market psychology** behind the morning star pattern is straightforward: After a steep sell-off (Day 1), the market finds a form of tentative equilibrium (Day 2). This could be due to shorts taking profit or buyers testing the waters at lower prices, resulting in a session with a small range and indecision. The “star” on Day 2 reflects how the bears’ strength is waning. Then on Day 3, the bulls make a definitive stand – the large upward candle shows **buying resurgence and a shift in sentiment from bearish to bullish**. Traders interpret this as a sunrise after the dark night: a new uptrend may be starting. The presence of the small middle candle is crucial because it differentiates the pattern from a simple two-day reversal; it shows that the momentum didn’t flip directly but rather went through a phase of neutralization before reversing. This often makes the morning star more reliable, as it indicates the downtrend’s momentum was truly halted before reversing. Confirmation in the form of volume (higher volume on Day 3) or subsequent price strength (e.g., Day 4 making a higher high) can further validate the signal.

### Backtrader Implementation

Implementing a morning star detection in code involves looking back over the last 3 bars on each new bar and checking the pattern conditions. Below is a simple Backtrader strategy that identifies morning star patterns and enters a long position when one is found. As before, we use daily data from the `pwb-toolbox`. This example will focus strictly on the three-bar formation without additional filters for trend or volume, for clarity. (Note: Morning stars are relatively rare, so depending on the data length, you may see few signals. They tend to be more significant on higher timeframes like daily charts and in major instruments.)

```python
# Morning Star Candlestick Pattern Trading Strategy
import backtrader as bt
import pwb_toolbox.datasets as pwb_ds

class MorningStarStrategy(bt.Strategy):
    def next(self):
        # Need at least 3 bars to form the pattern
        if len(self.data) < 3:
            return
        # Retrieve the last three bars (indices -2, -1, 0 relative to current bar)
        open1, high1, low1, close1 = self.data.open[-2], self.data.high[-2], self.data.low[-2], self.data.close[-2]
        open2, high2, low2, close2 = self.data.open[-1], self.data.high[-1], self.data.low[-1], self.data.close[-1]
        open3, high3, low3, close3 = self.data.open[0],  self.data.high[0],  self.data.low[0],  self.data.close[0]
        # Check Morning Star conditions:
        # Day 1: bearish (long red candle assumed)
        if close1 < open1:
            # Day 2: small body (near doji) - here we require body2 smaller than half of body1
            body1 = abs(close1 - open1)
            body2 = abs(close2 - open2)
            if body2 < 0.5 * body1:
                # (Optional gap check: ensure day2 is below day1's close)
                # if high2 < close1:
                # Day 3: bullish and closes above midpoint of day1
                if close3 > open3 and close3 >= (open1 + close1) / 2:
                    self.buy()

# Load daily data (AAPL for example)
df = pwb_ds.load_dataset("Stocks-Daily-Price", ["AAPL"])
data = bt.feeds.PandasData(dataname=df)
# Run the backtest with MorningStarStrategy
cerebro = bt.Cerebro()
cerebro.addstrategy(MorningStarStrategy)
cerebro.adddata(data)
cerebro.run()
```

This strategy inspects the three most recent bars whenever a new bar comes in. The code first ensures we have at least 3 data points. It then assigns variables for the open, high, low, close of the potential pattern: `-2` corresponds to Day 1 (two bars ago), `-1` to Day 2 (previous bar), and `0` to Day 3 (current bar). The conditions checked are:

* Day 1 bearish: `close1 < open1`. (We assume Day 1 is a significantly long candle; in code we didn’t enforce length explicitly besides later comparing to Day 2’s body.)
* Day 2 small body: We require `body2 < 0.5 * body1` as a simple way to ensure the second candle is much smaller than the first. In a more refined approach, we might also ensure Day 2’s range is below Day 1’s close (e.g., `high2 < close1`) to simulate the gap – this is commented out above and can be enabled if analyzing assets that do gap.
* Day 3 bullish and closes above Day 1 midpoint: `close3 > open3` and `close3 >= (open1 + close1)/2`. If these conditions are satisfied, the pattern is recognized and `self.buy()` executes a buy.

We did not incorporate every nuance (such as explicitly checking a gap down on Day 2 or a gap up on Day 3) because not all markets gap, and Backtrader data might not show gaps if using continuous pricing. However, the core logic captures the essence of a morning star: big down, small hesitation, big up.

In a robust strategy, one might add that the third day’s open (`open3`) is above the second day’s close (`close2`), as an additional sign of strength (gap up). Volume data could also be integrated – for example, requiring volume on Day 3 to exceed a moving average of volume – since a true morning star often has heavy volume on the reversal day. For exit strategy, a simple approach could be to hold the long position for a target profit or a fixed number of days, or use a trailing stop, but those rules are beyond the scope of pattern identification. The above implementation is a straightforward template for detecting morning stars in a historical dataset using Backtrader.

## Conclusion

**Bullish candlestick patterns** like the Bullish Engulfing, Hammer, and Morning Star can indeed be encoded into algorithmic trading strategies and have shown **quantifiable predictive power** in certain backtests. Using a framework like Backtrader along with comprehensive datasets (such as those in the pwb-toolbox) allows traders to **backtest** these patterns objectively over decades of historical data. For example, one data-driven study on S\&P 500 stocks found the Bullish Engulfing had about a *74% win rate* and an average gain of \~0.3% per trade, while the Piercing Line (a similar two-day pattern) showed an *81% win rate* with \~0.5% average gains. The Hammer pattern is often touted as highly reliable and in tests produced a win rate around 76%, though with a smaller profit factor. The Morning Star, being rarer, is generally considered a strong bullish signal when it appears, and some sources estimate its historical success rate in the \~60% range – though its performance can vary widely by market and definition criteria.

However, it’s important to approach these patterns with a **critical mindset**. The edges they provide tend to be modest; as the above statistics imply, the average price move following a “successful” pattern might be only a fraction of a percent. Such small edges can be easily eroded by transaction costs, slippage, or unfavorable market conditions. Moreover, pattern performance is **context-dependent**. A bullish pattern appearing during a strong bearish macro-trend may fail frequently. This is why traders often enhance candlestick strategies with **filters** – for instance, only taking a Bullish Engulfing if a longer-term trend indicator is oversold, or requiring confirmation (like a higher close the next day) before entry. Studies have noted that combining candlestick signals with trend or momentum filters can improve their effectiveness.

**Backtesting reliability** also hinges on precise definitions. One must define the candlestick pattern rules unambiguously (as we did with mathematical conditions) to avoid subjective interpretation. It’s easy to “see” a pattern on a chart after the fact, but an algorithm needs exact thresholds for what counts as, say, a long shadow or a small body. Slight variations in these definitions can change the backtest results. Thus, thorough testing across different instruments and time periods is recommended to ensure a pattern’s viability wasn’t a fluke in a particular dataset.

Additionally, while our examples executed immediate trades on pattern signals, many practitioners use **confirmatory signals** to boost probabilities – for example, waiting for the next candle to trade above the hammer’s high (confirmation of bullish momentum) or using volume spikes to validate a Morning Star. Implementing stop-loss orders (e.g., below the pattern’s low) and profit targets is prudent risk management when trading these setups, as not every signal will lead to a sustained rally.

In summary, **bullish candlestick patterns** can “work” in algorithmic trading if applied with diligence: they encapsulate valuable information about shifts in buyer/seller dominance, and when rigorously defined they have shown **statistical edges** above random in historical data. The Backtrader implementations provided here demonstrate how to turn these chart patterns into testable trading rules. Nonetheless, one must be mindful of the **limitations** – no pattern is a guarantee of success. Proper backtesting (with out-of-sample validation), risk management, and perhaps the inclusion of additional technical criteria should accompany any strategy based on candlestick signals. With those caveats in place, these three bullish patterns remain popular tools in the algo trader’s arsenal for identifying potential trend reversals and timing **long entries** in a systematic way.


## References & Further Reading

[1]: Bergstra, J., Bardenet, R., Bengio, Y., & Kégl, B. (2011). ["Algorithms for Hyper-Parameter Optimization."](https://papers.nips.cc/paper/4443-algorithms-for-hyper-parameter-optimization) Advances in Neural Information Processing Systems 24.

[2]: ["Advances in Financial Machine Learning"](https://www.amazon.com/Advances-Financial-Machine-Learning-Marcos/dp/1119482089) by Marcos Lopez de Prado

[3]: ["Evidence-Based Technical Analysis: Applying the Scientific Method and Statistical Inference to Trading Signals"](https://www.amazon.com/Evidence-Based-Technical-Analysis-Scientific-Statistical/dp/0470008741) by David Aronson

[4]: ["Machine Learning for Algorithmic Trading"](https://github.com/PacktPublishing/Machine-Learning-for-Algorithmic-Trading-Second-Edition) by Stefan Jansen

[5]: ["Quantitative Trading: How to Build Your Own Algorithmic Trading Business"](https://books.google.com/books/about/Quantitative_Trading.html?id=j70yEAAAQBAJ) by Ernest P. Chan