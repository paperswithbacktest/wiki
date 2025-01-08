---
title: "Jeremy Perlow: Biography and Contributions (Algo Trading)"
description: "Jeremy Perlow is a key figure in futures and algo trading known for pioneering tech-driven market strategies enhancing trading efficiency and education."
---

Jeremy Perlow is a prominent name in the industry of futures trading and algorithmic trading. Over the course of several decades, he has established himself as an influential member of the trading community, having a formidable impact on trading practices and technology. Perlow's career has been characterized by a remarkable transition from a floor broker to an innovative business leader. This trajectory offers valuable insights into the dynamic nature and evolution of trading methodologies.

Perlow's career began during a significant era for financial markets, marked by technological advancements and regulatory changes. This period saw a shift from traditional open outcry trading systems to more sophisticated electronic trading platforms. Throughout his journey, Perlow embraced these changes, contributing to the development and adoption of algorithmic trading. His initiatives in creating efficient trading systems have been essential in enhancing market access and liquidity, thereby shaping modern trading strategies.

![Image](images/1.png)

Perlow's transition from floor broker to business leader was not merely a career progression; it was a reflection of his ability to adapt and innovate within an evolving market landscape. His work has not only strengthened the profitability and resilience of trading practices but has also provided educational resources through mentorship and training in algorithmic trading. Thus, Jeremy Perlow represents the merger of traditional financial expertise with cutting-edge technological solutions, making a lasting impact on the world of futures and algorithmic trading.

## Table of Contents

## Early Life and Education

Jeremy Perlow was born and raised in Highland Park, Illinois, a suburban city located in the greater Chicago metropolitan area known for its affluent community and high-quality educational institutions. From a young age, Perlow demonstrated a keen interest in the financial and business sectors, which would inevitably guide his future career path.

He completed his high school education at Glenbrook North High School, situated in Northbrook, Illinois. Glenbrook North is renowned for its robust academic programs and a strong emphasis on extracurricular activities, providing Perlow with a well-rounded educational foundation. During his time there, Perlow was likely involved in various academic and extracurricular pursuits that helped hone his analytical skills and business acumen.

Following his high school graduation, Perlow pursued higher education at Arizona State University (ASU), [earning](/wiki/earning-announcement) a degree focused on Business and Economics. ASU is noted for its diverse academic offerings and vibrant campus life, which supports an immersive learning experience. The university's business program, in particular, is recognized for integrating real-world business challenges into the curriculum, offering students practical insights into the workings of economic and financial systems. This academic environment would have provided Perlow with both theoretical knowledge and practical skills, forming a crucial foundation for his subsequent career in futures and algorithmic trading.

## Professional Journey

Jeremy Perlow began his professional journey in the trading industry alongside his father at the Chicago Mercantile Exchange (CME) in 1982. This period marked his initial exposure to the world of futures trading, where he would eventually leave a lasting impact. By 1988, Perlow advanced to the position of floor broker, specializing in the Dmark pit. This role was instrumental in shaping his early professional trajectory, offering him a deep understanding of the intricacies of futures trading.

During his tenure as a floor broker, Perlow honed his skills in executing trades and managing risks, which set the foundation for his later accomplishments. His proficiency in these areas was recognized by various entities in the trading sector, leading him to more significant roles. Among these roles, he notably served as a branch manager at Sweet Futures, where he demonstrated leadership and strategic decision-making abilities critical for fostering growth and innovation within the firm.

Perlow's career trajectory continued its upward trend as he assumed the position of CEO at JAIR Trading. In this capacity, he spearheaded various initiatives that underscored the importance of integrating traditional trading strategies with emerging technological advancements. His leadership at JAIR Trading was characterized by a focus on enhancing trading efficiencies and leveraging algorithmic solutions, which positioned the firm as a competitive player in the market.

Through these experiences, Perlow established a reputation as a forward-thinking leader in the trading community. His professional journey serves as a testament to the evolution of trading practices, illustrating the shift from traditional floor-based trading to the adoption of sophisticated electronic trading systems.

## Achievements in Algo Trading

Jeremy Perlow has been a key figure in the development of electronic trading systems, significantly enhancing the profitability of trading operations. His deep understanding of algorithmic and automated trading has allowed him to create innovative strategies that align with market demands. The transition from traditional to electronic trading has necessitated a paradigm shift, and Perlow has been at the forefront of this evolution.

His involvement in [algorithmic trading](/wiki/algorithmic-trading) is marked by the creation of systems that utilize complex mathematical models and computer algorithms to analyze market data and execute trades at optimal prices. Such systems have minimized human error and increased trading efficiency. Algorithmic trading utilizes a variety of strategies, including [trend following](/wiki/trend-following), statistical [arbitrage](/wiki/arbitrage), [market making](/wiki/market-making), and mean reversion. The implementation of these strategies often involves the analysis of historical data using statistical methods to identify patterns and trends that can be exploited for profit.

Perlow's contributions extend beyond system development; he has played a crucial role in mentoring new traders. Recognizing the challenges traders face when adapting to technological advancements, he has been involved in educational programs aimed at demystifying algorithmic and automated trading. These initiatives help traders understand complex algorithms and their applications, ultimately fostering a generation of skilled professionals adept at navigating modern trading environments.

Python, a versatile programming language frequently used in algorithmic trading, enables the development of algorithms for financial analysis. Perlow's work likely involves the use of Python for [backtesting](/wiki/backtesting) trading strategies, analyzing market trends, and optimizing trade execution. For example, a simple moving average crossover strategy in Python could be implemented as follows:

```python
import pandas as pd
import numpy as np

# Load market data
data = pd.read_csv('market_data.csv')
data['SMA50'] = data['Close'].rolling(window=50).mean()
data['SMA200'] = data['Close'].rolling(window=200).mean()

# Generate trading signals
data['Signal'] = np.where(data['SMA50'] > data['SMA200'], 1, 0)
data['Position'] = data['Signal'].diff()

# Evaluate strategy performance
initial_capital = 10000
positions = 10 * data['Position']  # number of stocks
portfolio = positions * data['Close']
portfolio['Cash'] = initial_capital - (positions * data['Close']).cumsum()
portfolio['Total'] = portfolio['Cash'] + (positions * data['Close'])
```

This example highlights Perlow's focus on utilizing algorithmic trading to maximize profit while minimizing risks. His achievements in the field underscore his pivotal role in the advancement of trading strategies, bridging the gap between traditional methodologies and modern technologies.

## Contribution to the CME

Throughout his career, Jeremy Perlow has demonstrated a strong commitment to the Chicago Mercantile Exchange (CME), contributing significantly to its development and innovation. His involvement with the CME encompasses both operational and strategic roles that have helped shape the institution's trajectory in a rapidly evolving trading environment.

Perlow's active participation in the CME is exemplified by his service on the CME Communication Committee and the New Technology Committee. These committees are crucial for maintaining robust communication channels within the organization and ensuring the institution remains at the forefront of technological innovation. His presence on these committees underscores his ability to bridge the gap between traditional trading practices and emerging technological trends, facilitating the progression of the CME's infrastructure and services.

Moreover, Perlow’s influence and dedication to the CME are further highlighted by his multiple nominations for the CME board of governors. This acknowledgment by his peers signals not only esteem for his expertise and vision but also trust in his leadership capabilities in guiding the CME through transformative phases in the trading sector.

His commitment to the CME has been pivotal in aligning the exchange's strategies with modern market demands. In addition to his formal roles, Perlow's insights into algorithmic trading and electronic trading systems have likely influenced broader policy and strategic discussions at the CME, ensuring the exchange's operations are in step with cutting-edge trading methodologies.

## Other Ventures and Interests

Jeremy Perlow has expanded his professional scope beyond trading to include successful ventures in technology and the food industry. He co-founded GXWEB, a web development company, where he played a crucial role as Chief Technology Officer (CTO). In this capacity, Perlow utilized his technical expertise to oversee the development of web solutions, enabling businesses to leverage online platforms effectively. His involvement in GXWEB underscores his ability to integrate technology across various sectors, identifying and capitalizing on digital trends before they became mainstream.

In addition to his accomplishments in web development, Perlow ventured into the spot market procurement business, focusing on commodities like cheese and butter. His enterprise served large corporations by offering streamlined procurement solutions tailored to the distinct needs of the food industry. This endeavor highlights Perlow's adaptability and keen business acumen, as he managed to cater to an entirely different market segment compared to his trading roots.

Moreover, Perlow contributed his insights as a freelance writer for The Meyers Report, a publication that covers various topics, including food and technology. His articles provided valuable perspectives on industry trends, bridging his interests in both trading and emerging technologies. Through these contributions, Perlow shared his knowledge and experiences, enhancing the dialogue within these sectors and solidifying his reputation as a multifaceted professional.

## Legacy and Impact

Jeremy Perlow's career embodies a harmonious integration of traditional trading methodologies with modern technological innovations. His influence extends across the financial landscape, where his pioneering efforts in algorithmic trading have not only spurred profitability but also propelled the industry toward a seamless fusion of human intuition and machine precision.

A key aspect of Perlow's legacy is his commitment to advancing educational initiatives within the trading community. By engaging in mentorship programs and developing comprehensive curricula, he has equipped numerous future traders with the necessary skills to navigate the complexities of algorithmic trading. This dedication to education ensures that his insights continue to benefit new generations, fostering an informed and adaptable trading community.

Perlow's work is characterized by a keen understanding of both the theoretical and practical aspects of electronic trading systems. His strategies often incorporated systematic approaches that optimize trading decisions based on quantitative analyses. These innovations have contributed significantly to the efficiency and effectiveness of market operations, setting benchmarks for best practices in the industry.

Moreover, his active participation in influential committees at the Chicago Mercantile Exchange (CME) demonstrated his foresight in technological advancements and market communication strategies. His role in shaping policies and standards at the CME further underscores his impact, as these efforts facilitated smoother transitions into electronic trading and enhanced market integrity.

Jeremy Perlow's legacy is a testament to the transformative power of integrating technology with traditional trading knowledge. His work continues to inspire industry professionals, encouraging them to embrace technological advancements while valuing the foundational principles of trading. Through his contributions, Perlow has indelibly marked the landscape of futures and algorithmic trading, bridging the past with the future in a rapidly evolving financial world.

## References & Further Reading

[1]: [Bergstra, J., Bardenet, R., Bengio, Y., & Kégl, B. (2011). "Algorithms for Hyper-Parameter Optimization."](https://dl.acm.org/doi/10.5555/2986459.2986743) Advances in Neural Information Processing Systems 24.

[2]: ["Advances in Financial Machine Learning"](https://www.amazon.com/Advances-Financial-Machine-Learning-Marcos/dp/1119482089) by Marcos Lopez de Prado

[3]: ["Evidence-Based Technical Analysis: Applying the Scientific Method and Statistical Inference to Trading Signals"](https://onlinelibrary.wiley.com/doi/book/10.1002/9781118268315) by David Aronson

[4]: ["Machine Learning for Algorithmic Trading"](https://github.com/stefan-jansen/machine-learning-for-trading) by Stefan Jansen

[5]: ["Quantitative Trading: How to Build Your Own Algorithmic Trading Business"](https://www.amazon.com/Quantitative-Trading-Build-Algorithmic-Business/dp/1119800064) by Ernest P. Chan