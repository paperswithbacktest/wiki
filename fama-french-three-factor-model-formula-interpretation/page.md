---
title: "Fama-French Three-Factor Model: Formula and Interpretation"
description: "Explore the Fama-French Three-Factor Model's role in algorithmic trading. Learn how this model enhances portfolio performance by leveraging size and value factors."
---


![Image](images/1.png)

## Table of Contents

## What is the Fama-French Three-Factor Model?

The Fama-French Three-Factor Model is a way to understand why some stocks do better than others. It was created by Eugene Fama and Kenneth French. The model says that stock returns are affected by three main things: the overall market, the size of the company, and the company's book-to-market ratio. The market part is easy to understand: if the whole stock market goes up, most stocks go up too. The size part means that smaller companies often do better than bigger ones. The book-to-market ratio part means that companies with high book values compared to their market values tend to do better.

This model helps investors and researchers see why some stocks perform the way they do. It's more detailed than just looking at the market as a whole. By considering the size of the company and its book-to-market ratio, the model can explain more about stock returns than just using the market alone. This is useful for people who want to pick stocks or understand the stock market better. The Fama-French model has been very influential and is widely used in finance.

## Who developed the Fama-French Three-Factor Model?

The Fama-French Three-Factor Model was developed by Eugene Fama and Kenneth French. Eugene Fama is a famous economist who won the Nobel Prize in Economics. Kenneth French is also a well-known economist and a professor. They worked together to create this model to help explain why some stocks do better than others.

They came up with this model because they wanted to understand stock returns better than just looking at the overall market. They found that three things were important: the market, the size of the company, and the book-to-market ratio. This model helps investors and researchers see why stocks perform the way they do. It's been very helpful and is used a lot in finance.

## What are the three factors in the Fama-French model?

The Fama-French Three-Factor Model looks at three things that can affect how well stocks do. The first factor is the market. This means that if the whole stock market goes up or down, most stocks will follow that trend. It's like the tide that lifts or lowers all boats. The second factor is the size of the company. Smaller companies often do better than bigger ones. This might be because smaller companies can grow faster or because investors see more potential in them.

The third factor is the book-to-market ratio. This is a bit more complicated, but it's about comparing what a company is worth on paper (its book value) to what investors are willing to pay for it in the market (its market value). Companies with a high book-to-market ratio, meaning their book value is high compared to their market value, tend to do better. This could be because these companies are seen as undervalued or because they might be in a better position to grow. These three factors together help explain why some stocks perform better than others.

## How does the Fama-French model differ from the Capital Asset Pricing Model (CAPM)?

The Fama-French Three-Factor Model and the Capital Asset Pricing Model (CAPM) both aim to explain why stocks perform the way they do, but they do it in different ways. The CAPM is simpler and looks at just one thing: how the stock moves with the overall market. It says that a stock's return depends on how risky it is compared to the market. If a stock moves a lot when the market moves, it's riskier and should give a higher return to make up for that risk.

The Fama-French model, on the other hand, is more detailed. It looks at three things instead of just one: the market, the size of the company, and the book-to-market ratio. It says that smaller companies and companies with high book-to-market ratios tend to do better than others. This model tries to explain more about why some stocks do better than others by looking at these extra factors. So, while the CAPM focuses on market risk, the Fama-French model adds in the effects of company size and value to give a fuller picture of stock returns.

## What is the formula for the Fama-French Three-Factor Model?

The Fama-French Three-Factor Model has a formula that helps figure out how well a stock does. The formula is: R_i - R_f = α_i + β_i(MKT - R_f) + s_i(SMB) + h_i(HML) + ε_i. Here, R_i is the return of the stock, R_f is the risk-free rate (like what you'd get from a safe investment like a government bond), MKT is the return of the overall market, SMB stands for "Small Minus Big" and looks at the size of the company, and HML stands for "High Minus Low" and looks at the book-to-market ratio. The letters α, β, s, and h are numbers that show how much each part affects the stock's return, and ε is an error term that shows other stuff that might affect the return.

This formula helps break down why a stock might do better or worse than expected. The first part, β_i(MKT - R_f), is similar to the Capital Asset Pricing Model and shows how the stock moves with the market. The second part, s_i(SMB), shows how much the size of the company matters. If s_i is positive, it means smaller companies do better. The third part, h_i(HML), shows how much the book-to-market ratio matters. If h_i is positive, it means companies with high book-to-market ratios do better. By looking at these three things together, the Fama-French model gives a more detailed picture of what affects stock returns.

## How are the market, size, and value factors calculated in the Fama-French model?

In the Fama-French model, the market factor is calculated by looking at the difference between the return of the overall market and the risk-free rate. The overall market return can be measured by a broad market index like the S&P 500. The risk-free rate is usually the return on a safe investment like a government bond. So, if the market goes up more than the risk-free rate, the market factor is positive, and if it goes up less, it's negative. This helps show how much the stock moves with the market.

The size factor, or SMB (Small Minus Big), is calculated by looking at the difference in returns between small companies and big companies. To do this, companies are sorted into groups based on their market capitalization, which is the total value of their stock. The returns of the smallest companies are compared to the returns of the biggest companies. If small companies do better than big ones, the size factor is positive, showing that smaller companies are doing better.

The value factor, or HML (High Minus Low), is calculated by looking at the difference in returns between companies with high book-to-market ratios and those with low book-to-market ratios. The book-to-market ratio is the company's book value divided by its market value. Companies are sorted into groups based on this ratio. The returns of companies with high book-to-market ratios are compared to the returns of companies with low book-to-market ratios. If companies with high book-to-market ratios do better, the value factor is positive, showing that value stocks are doing better than growth stocks.

## What does each factor in the Fama-French model represent?

The market factor in the Fama-French model shows how a stock moves with the overall stock market. It's calculated by taking the return of the whole market, like the S&P 500, and subtracting the return of a safe investment, like a government bond. If the market goes up more than the safe investment, the market factor is positive, which means the stock is doing well when the market does well. If the market goes up less than the safe investment, the market factor is negative, showing the stock isn't doing as well as the market.

The size factor, called SMB (Small Minus Big), looks at how the size of a company affects its stock returns. It's found by comparing the returns of small companies to the returns of big companies. Companies are sorted by their total value, or market capitalization. If small companies do better than big ones, the size factor is positive, which means smaller companies are doing better. This helps investors see if smaller companies are a good investment.

The value factor, called HML (High Minus Low), looks at how the book-to-market ratio of a company affects its stock returns. The book-to-market ratio is what the company is worth on paper (book value) divided by what investors are willing to pay for it (market value). Companies are sorted by this ratio. If companies with high book-to-market ratios do better than those with low ratios, the value factor is positive. This shows that stocks that are seen as undervalued or have more room to grow are doing better.

## How can the Fama-French model be used to evaluate investment portfolios?

The Fama-French model can help investors understand and evaluate their investment portfolios by looking at three important factors: the market, the size of companies, and the value of companies. By using the model, investors can see how their portfolio is doing compared to these three factors. For example, if an investor's portfolio has a lot of small companies, the size factor (SMB) will show if those small companies are doing better or worse than big companies. This can help the investor decide if they want to keep investing in small companies or switch to bigger ones.

The model also helps investors see if their portfolio is doing well because of the overall market, the size of the companies they own, or the value of those companies. If the market factor (MKT) is high, it means the portfolio is doing well because the whole market is doing well. If the value factor (HML) is high, it means the portfolio is doing well because the companies in it have high book-to-market ratios. By understanding these factors, investors can make better choices about which stocks to buy or sell to improve their portfolio's performance.

## What are some practical applications of the Fama-French Three-Factor Model in finance?

The Fama-French Three-Factor Model is really useful in finance for figuring out why some stocks do better than others. It helps investors and financial experts understand if their investments are doing well because of the overall market, the size of the companies they own, or the value of those companies. For example, if someone's portfolio has a lot of small companies, the model can show if those small companies are doing better or worse than big companies. This can help the investor decide if they should keep investing in small companies or switch to bigger ones. By looking at these three factors, investors can make smarter choices about which stocks to buy or sell to make their portfolio perform better.

Another way the Fama-French model is used in finance is for building better investment strategies. Financial experts can use the model to create portfolios that are balanced across the market, size, and value factors. This can help reduce risk and improve returns. For example, if a portfolio is too focused on big companies, the model might suggest adding some small companies to balance it out. Or if a portfolio has too many growth stocks, the model might suggest adding some value stocks to improve performance. By using the Fama-French model, financial experts can design portfolios that are more likely to succeed in the long run.

## How has the performance of the Fama-French model been empirically tested?

The Fama-French Three-Factor Model has been tested a lot to see if it really works. Researchers have looked at a lot of stock data from different times and places to check if the model can explain why some stocks do better than others. They've found that the model does a good job of explaining stock returns, especially when it comes to the size and value factors. Studies have shown that smaller companies and companies with high book-to-market ratios often do better than others, just like the model says. This has made the model very popular and trusted in finance.

But, the model isn't perfect. Some researchers have pointed out that it doesn't work as well for all markets or all times. For example, it might work better in the U.S. than in other countries. Also, some studies have found that other factors, like how much a company invests or how profitable it is, might also affect stock returns. Even so, the Fama-French model is still seen as a very useful tool for understanding stock returns and helping investors make better choices.

## What are the criticisms and limitations of the Fama-French Three-Factor Model?

The Fama-French Three-Factor Model has some criticisms and limits. One big criticism is that it doesn't work the same in all places or times. For example, it might explain stock returns better in the U.S. than in other countries. Also, some people think the model doesn't look at all the things that can affect stock returns. They say things like how much a company invests or how profitable it is might be important too. These other factors could make the model better if they were included.

Another limit is that the model can be hard to use in real life. It needs a lot of data and math to work right, which can be tough for regular investors. Also, the model looks at past data to predict the future, but the stock market can change a lot. What worked in the past might not work in the future. So, while the model is useful, it's not perfect and investors should be careful when using it to make choices about their investments.

## How have extensions and modifications to the Fama-French model been developed to address its limitations?

To address the limitations of the Fama-French Three-Factor Model, Eugene Fama and Kenneth French came up with a new version called the Five-Factor Model. This new model adds two more factors to the original three: profitability and investment. The profitability factor looks at how much profit a company makes, and the investment factor looks at how much a company invests in itself. By adding these two factors, the model can explain more about why some stocks do better than others. It helps investors see if companies that make more profit or invest more in themselves tend to do better in the stock market.

Other researchers have also tried to improve the Fama-French model by adding their own factors. For example, some have added a momentum factor, which looks at whether stocks that have been going up keep going up. Others have added a liquidity factor, which looks at how easy it is to buy and sell a stock. These extra factors can help make the model work better in different markets and times. But, adding more factors also makes the model more complicated to use. So, while these extensions and modifications try to fix the model's limits, they also make it harder for regular investors to use without a lot of help.

## What is the Fama-French Three-Factor Model and how can it be understood?

The Fama-French Three-Factor Model, introduced in 1992 by Eugene F. Fama and Kenneth R. French, enhances the Capital Asset Pricing Model (CAPM) by incorporating additional factors beyond the traditional market risk. CAPM primarily accounts for a single factor—market risk, represented by the beta of the security. However, empirical research suggested that other factors, such as company size and value characteristics, also influence stock returns. The Fama-French model addresses these discrepancies by introducing two additional factors: Size (SMB - Small Minus Big) and Value (HML - High Minus Low).

The model is mathematically expressed as follows:

$$
R_i = R_f + \beta (R_m - R_f) + s \times SMB + h \times HML + \epsilon
$$

where:
- $R_i$ is the expected return of the portfolio or asset.
- $R_f$ is the risk-free rate.
- $R_m$ is the market return.
- $\beta$ represents the sensitivity of the asset to market movements.
- $s$ and $h$ are coefficients determined through regression analysis that represent the sensitivity to the size and value factors, respectively.
- $\epsilon$ is the residual error term.

**Market Risk Factor** (Market Beta): Just like in CAPM, this factor represents the risk associated with the overall market. It measures how the stock or portfolio returns move relative to market returns.

**Size Factor (SMB - Small Minus Big)**: This factor captures the historical tendency for stocks of small-cap firms to outperform those of large-cap firms. The SMB factor is calculated as the difference between the returns of a portfolio of small-cap stocks and a portfolio of large-cap stocks. The premise is that smaller companies, often underrepresented in large indexes, may offer higher potential returns due to their growth opportunities and comparatively higher risk.

**Value Factor (HML - High Minus Low)**: The value factor accounts for the empirical anomaly where stocks with a high book-to-market ratio (value stocks) tend to outperform those with a low book-to-market ratio (growth stocks). HML is calculated by subtracting the returns of a portfolio of low book-to-market stocks from a portfolio of high book-to-market stocks. Value stocks, often undervalued by the market, could potentially yield higher returns as the market corrects their valuation.

The inclusion of these factors provides a more nuanced analysis of asset returns, challenging the CAPM assumption that market risk is the sole determinant. By acknowledging that size and value significantly affect returns, the Fama-French model offers an enhanced framework for investors and academics to evaluate and predict stock performance. It aids in explaining the variations in returns that CAPM could not, particularly for diversified portfolios encompassing different market segments.

## What is the Case Study about Applying the Fama-French Model?

A practical example of applying the Fama-French Three-Factor Model involves evaluating AT&T stocks within a trading system. This case study compares model-driven strategies against traditional buy-and-hold approaches, focusing on enhancing returns through strategic decision-making.

The Fama-French model, by incorporating the market risk, size, and value factors, allows for the development of trading strategies that are well-grounded in historical data analysis. In this case study, we implement trading strategies using Python, leveraging its libraries for data processing and statistical analysis.

First, historical price data of AT&T stocks is obtained, and necessary preprocessing steps are executed using Python's Pandas library. The regression model based on the Fama-French factors is then constructed to forecast future returns. The model is represented by the equation:

$$
R_i = \alpha + \beta_1(R_m - R_f) + \beta_2 \times \text{SMB} + \beta_3 \times \text{HML} + \epsilon
$$

Where:
- $R_i$ is the return of AT&T stocks,
- $R_m - R_f$ is the market risk premium,
- SMB (Small Minus Big) is the size factor,
- HML (High Minus Low) is the value factor,
- $\alpha$ and $\beta$s are coefficients to be determined.

Python's Statsmodels library is employed for performing regression analysis, allowing for the derivation of these coefficients. The strategies developed based on this model are then backtested against traditional buy-and-hold techniques using risk-adjusted return metrics such as the Sharpe Ratio and Sortino Ratio.

The Sharpe Ratio is calculated as follows:

$$
\text{Sharpe Ratio} = \frac{\overline{R_i - R_f}}{\sigma_i}
$$

Where:
- $\overline{R_i - R_f}$ is the average excess return,
- $\sigma_i$ is the standard deviation of the return.

Similarly, the Sortino Ratio is computed to account for downside risk, providing further insights into the performance of the strategies:

$$
\text{Sortino Ratio} = \frac{\overline{R_i - R_f}}{\sigma_d}
$$

Where:
- $\sigma_d$ is the standard deviation of negative returns.

The case study revealed that model-driven strategies could potentially offer superior returns under suitable market conditions, as evidenced by higher Sharpe and Sortino Ratios compared to the buy-and-hold strategy. This suggests that integrating the Fama-French model into algorithmic trading systems, especially using robust programming tools like Python, can enhance portfolio performance by better understanding and predicting stock returns.

## What is the conclusion?

The Fama-French Three-Factor Model stands as a vital tool for algorithmic traders aiming to decode the complexities of stock market returns. By enriching the traditional Capital Asset Pricing Model with size and value factors, it provides deeper insights into the intrinsic dynamics of market behavior. These insights allow traders to craft portfolios that are not only diversified but also resilient to market fluctuations.

The model's strength lies in its ability to isolate factors like market risk, size premium, and value premium, represented mathematically as:

$$
R_i = R_f + \beta_i (R_m - R_f) + s_i \times SMB + h_i \times HML + \epsilon_i
$$

where $R_i$ is the expected return on the stock, $R_f$ is the risk-free rate, $\beta_i$ is the sensitivity to market risk, $SMB$ (Small Minus Big) and $HML$ (High Minus Low) capture the size and value effects, respectively, and $\epsilon_i$ represents the residual error.

Despite its comprehensive nature, traders need to approach the model's predictions with caution. Given that it predominantly relies on historical data, the assumptions may not account for abrupt market changes and macroeconomic shocks. Thus, integrating real-time data and additional predictive factors is recommended to enhance the model's robustness.

To sustain a competitive edge, continuous evaluation and adaptation of strategies based on the model are indispensable. Algorithmic traders should ensure their systems are agile, allowing for modifications as new data and trends emerge. By doing so, they can maintain effective market positioning and optimize returns.

## References & Further Reading

Fama, E. F., & French, K. R. (1993). "Common risk factors in the returns on stocks and bonds." Journal of Financial Economics. This seminal paper introduces the Fama-French Three-Factor Model, outlining the significance of size and value factors in explaining stock returns. It is foundational for finance professionals interested in understanding market behavior beyond the Capital Asset Pricing Model (CAPM).

Carhart, M. M. (1997). "On Persistence in Mutual Fund Performance." The Journal of Finance. This study expands on the Fama-French model by considering [momentum](/wiki/momentum) as an additional factor in asset pricing. It is valuable for those exploring enhancements to the original three-factor framework.

Jegadeesh, N., & Titman, S. (1993). "Returns to Buying Winners and Selling Losers: Implications for Stock Market Efficiency." The Journal of Finance. This research highlights the momentum effect in stock markets, advocating for a strategy that capitalizes on past winners and sells past losers, enriching the discourse on market anomalies and efficiency.

Hilpisch, Y. "Python for Finance: Mastering Data-Driven Finance." This resource is excellent for practitioners interested in leveraging Python for financial analyses, providing practical insights into data management, backtesting, and implementation of financial models, including the Fama-French Three-Factor Model.

Gray, W. R., & Carlisle, T. E. "Quantitative Value: A Practitioner's Guide to Automating Intelligent Investment." This book offers a comprehensive guide to value investing through quantitative strategies, serving as a practical resource for implementing intelligent investment processes using models like Fama-French.

