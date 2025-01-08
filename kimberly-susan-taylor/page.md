---
title: "Kimberly Susan Taylor (Algo Trading)"
description: "Explore the remarkable contributions of Kimberly S. Taylor and Susan Taylor in algorithmic trading, revealing how they shaped modern financial practices."
---





This article provides a comprehensive exploration of two influential figures in the financial industry: Kimberly S. Taylor and Susan Taylor. Their contributions, particularly in the domain of algorithmic trading, have had a profound impact on modern financial practices. Kimberly S. Taylor is widely recognized for her significant tenure at the CME Group, where she led various departments and played a pivotal role in the organization's growth and stability. Her expertise in risk management and clearing has been instrumental, particularly during challenging financial periods.

On the other hand, Susan Taylor has made her mark through groundbreaking work in algorithmic trading, a field that has revolutionized how financial transactions are executed. Her innovative approaches have set new benchmarks for speed and efficiency in trading, thus solidifying her legacy in the industry.

This examination aims to highlight their backgrounds, professional achievements, and the challenges they overcame while shedding light on their lasting influence on the financial sector. Both Kimberly and Susan have contributed to shaping modern trading practices, leaving a lasting legacy that continues to inspire future generations of professionals in finance and trading.


## Table of Contents

## Early Life and Education of Kimberly S. Taylor

Kimberly S. Taylor was raised in Michigan, where she initially aspired to pursue a career in law. However, her career trajectory took a decisive turn towards business, as she chose to obtain an MBA from Eastern Michigan University in 1986. During this period, business schools were predominantly male environments, making her educational journey noteworthy for her distinction as one of the few women navigating the challenges and opportunities of a male-dominated academic field. Taylor's choice to pivot from law to business was not just a testament to her adaptability but also set the foundation for her future contributions to the financial industry. Her early life and education equipped her with a unique perspective and determination, pivotal for her eventual success in finance and trading.


## Professional Journey at CME Group

Kimberly S. Taylor commenced her career at the Chicago Mercantile Exchange (CME) as an analyst in 1989, embarking on a path that would see her rise to significant leadership positions within the organization. Her tenure at CME was characterized by a commitment to learning and development, which she pursued through various educational courses and volunteer opportunities. These activities allowed her to gain substantial insights into complex areas such as options pricing, a critical component of financial markets.

Taylor's ability to leverage educational resources and real-world applications played a crucial role in her rapid advancement within CME. By 2004, she had ascended to the position of president of CME Clearing. In this role, she was responsible for overseeing the division that manages counterparty credit risk for all trades occurring at the CME, a pivotal part of the financial institution's risk management framework.

Her leadership at CME Clearing was particularly significant during times of financial instability. Taylor adeptly guided the clearing division through several major crises, notably the collapse of Refco in 2005 and the failure of MF Global in 2011. These events posed considerable challenges due to the potential for systemic risk they introduced to the financial markets. Under Taylor's stewardship, CME Clearing implemented advanced risk management strategies to uphold market integrity and protect participant funds.

Taylor's strategic initiatives and decision-making were instrumental in maintaining the stability and trustworthiness of the clearing processes at CME. Her efforts not only safeguarded the exchange but also set new standards in crisis management for clearinghouses globally.


## Achievements and Recognition

Kimberly S. Taylor has been a formidable presence in the financial industry, recognized for her exceptional contributions to trading and risk management. Her induction into the Futures Industry Association's Futures Hall of Fame in 2019 is a testament to her influence and impact in the futures markets. This prestigious honor was earned through her leadership, notably during periods of financial turbulence where she was instrumental in navigating and managing counterparty risks—an essential aspect of maintaining stability and trust in financial exchanges.

As the president of CME Clearing, Taylor played a crucial role in innovating and implementing cross-margin programs. These programs were designed to optimize the use of collateral by traders, enhancing financial efficiency and reducing overall systemic risk. Cross-margining works by allowing traders to net positions across different markets, effectively lowering the margin requirements and, thus, their capital costs. This advancement not only improved the CME Group's offerings but also set new benchmarks for risk management processes in the industry.

In 2014, Crain's Chicago Business recognized Taylor as one of Chicago's most powerful women. This accolade highlights her prominent role in shaping the future of financial trading in one of the world's major economic hubs. Her strategic decision-making and innovation in risk management practices earned her widespread respect and admiration, further demonstrating the weight of her contributions to the financial sector.

Through her efforts, Kimberly S. Taylor has not only advanced her career but has also paved the way for greater efficiency and security in financial trading practices. Her leadership continues to serve as an example for professionals in the financial sector.


## Susan Taylor and the World of Algo Trading

Susan Taylor is a noteworthy figure in the domain of [algorithmic trading](/wiki/algorithmic-trading), having made significant strides that have shaped contemporary trading practices. Her groundbreaking work facilitated the automation and optimization of trading processes, fundamentally transforming how trades are executed with increased speed and efficiency.

Algorithmic trading leverages computer programs to automatically execute trades based on pre-defined criteria. Taylor's contributions to this field have been pivotal, particularly in enhancing the speed and precision of trade execution. These advancements allow for a more efficient market by reducing transaction costs and minimizing market impact during trades.

One of Taylor's key achievements was her involvement in developing algorithms that have set industry benchmarks. These algorithms are designed to analyze vast amounts of market data to identify optimal trading opportunities. This analysis often involves complex computational techniques and mathematical models. For instance, her work incorporated predictive modeling and [machine learning](/wiki/machine-learning) principles to improve decision-making processes in trading.

Moreover, Taylor's influence extends to the design of algorithms that prioritize risk management and compliance with regulatory standards. By integrating these considerations into trading algorithms, she ensured that automated trading systems adhere to legal guidelines while maintaining robust security measures.

In Python, the implementation of a simple moving average crossover strategy, an example of an algorithmic trading strategy, can illustrate the foundation of Taylor’s work:

```python
import pandas as pd

# Load market data
data = pd.read_csv('market_data.csv')

# Calculate moving averages
data['SMA_20'] = data['Close'].rolling(window=20).mean()
data['SMA_50'] = data['Close'].rolling(window=50).mean()

# Generate signals
data['Signal'] = 0
data.loc[data['SMA_20'] > data['SMA_50'], 'Signal'] = 1
data.loc[data['SMA_20'] < data['SMA_50'], 'Signal'] = -1

# Example of a signal for an entry or exit point
print(data[['Date', 'Close', 'SMA_20', 'SMA_50', 'Signal']].tail())
```

This code snippet represents a basic algorithmic trading concept that Taylor might have expanded upon. Throughout her career, Susan Taylor's innovative approaches have contributed to the increasingly prevalent role of algorithmic trading in financial markets. Her legacy continues to influence the development of sophisticated trading systems that capitalize on technological advancements to foster more efficient market environments.


## Impact on Modern Trading Practices

Kimberly S. Taylor's contributions to the financial industry, particularly in clearing and risk management at CME Group, have been instrumental in establishing new standards for crisis handling. Her leadership in CME Clearing during significant financial upheavals, such as the collapses of Refco and MF Global, emphasized the importance of robust clearing mechanisms and proactive risk management in maintaining market stability. Taylor's focus on managing counterparty risk and implementing innovative cross-margin programs provided financial safeguards that strengthened the resilience of financial markets. These measures have become industry benchmarks, influencing modern trading practices by prioritizing systemic risk reduction and enhancing the overall integrity of financial transactions.

Conversely, Susan Taylor's pioneering efforts in algorithmic trading have fundamentally transformed trade execution by leveraging technology to achieve unprecedented speed and efficiency. Her work in developing advanced trading algorithms has enabled sophisticated trading strategies that capitalize on market opportunities with precision and agility. Algorithmic trading, characterized by mathematical models and automated systems, facilitates rapid decision-making and execution, minimizing latency and human error. The algorithms Susan Taylor contributed to have become industry standards, steering the evolution of trading strategies and broadening the horizon for what can be achieved through technological advancements.

Together, the legacies of Kimberly and Susan Taylor significantly shape current financial markets. Kimberly's advancements in clearing protocols ensure stability during periods of market stress, while Susan's innovations in algorithmic trading promote faster, more efficient markets. These contributions underscore the pivotal role of leadership and technology in shaping modern trading practices, highlighting the ongoing need for strategic vision and innovation to drive financial market evolution.


## Conclusion

The combined efforts of Kimberly S. Taylor and Susan Taylor within the financial industry have sparked transformative changes, especially in clearing operations and algorithmic trading. Kimberly S. Taylor's leadership at CME Group marked a pivotal shift in how financial risk and crises are managed, setting new benchmarks in clearing and counterparty risk management. Her forward-thinking approaches not only fortified the stability and resilience of market mechanisms but also paved the way for future innovations in financial operations and risk assessment.

On the other hand, Susan Taylor's pioneering advancements in algorithmic trading have fundamentally altered trade execution processes. Her contributions to the development of sophisticated trading algorithms have enhanced the speed and accuracy of transactions, solidifying the reliability and efficiency of modern trading systems. This has enabled market participants to leverage technology more effectively, maximizing trading opportunities and outcomes.

Both Kimberly and Susan have thus established a legacy of excellence and ingenuity, illustrating the profound impact that visionary leadership and technological advancements can have in revolutionizing industry norms. Their careers serve as a testament to the significant role women play in shaping the evolution of finance, inspiring upcoming generations to explore and innovate within the trading landscape. Their achievements continue to highlight the critical importance of adaptation and progressive thinking in sustaining and enhancing the dynamic nature of financial markets.




## References & Further Reading

[1]: ["Advances in Financial Machine Learning"](https://www.amazon.com/Advances-Financial-Machine-Learning-Marcos/dp/1119482089) by Marcos Lopez de Prado

[2]: ["Building Financial Models"](https://www.theknowledgeacademy.com/blog/how-to-build-a-financial-model/) by John S. Tjia

[3]: ["Evidence-Based Technical Analysis: Applying the Scientific Method and Statistical Inference to Trading Signals"](https://www.amazon.com/Evidence-Based-Technical-Analysis-Scientific-Statistical/dp/0470008741) by David Aronson

[4]: ["Quantitative Trading: How to Build Your Own Algorithmic Trading Business"](https://www.amazon.com/Quantitative-Trading-Build-Algorithmic-Business/dp/1119800064) by Ernest P. Chan

[5]: ["High-Frequency Trading: A Practical Guide to Algorithmic Strategies and Trading Systems"](https://books.google.com/books/about/High_Frequency_Trading.html?id=6l0DDQAAQBAJ) by Irene Aldridge