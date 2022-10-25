# project-II-pipelines
Project_2_Pipelines

# Project: Data Pipeline
Test_1
## Overview

This project aims to test two combined APIs. The first API retrieves information from the Reddit site, while the second is an API that retrieves data from Yahoo Finance.

Thanks to the API using information from Reddit, the idea is to see if the stocks that have a high exposure on the platform follow in the following days the price that the market. 

## Selection of the stocks

After a first attempt to use the Reddit API, I could not retrieve the whole year's data as I initially wanted to, or I would quickly receive a 429 error. So I randomly selected five dates in the last five months and extracted the top 50 most popular stocks on those five dates. 

As expected on these five dates, 2 of the three stocks are of the same stock. The same stocks are defined as follows: Meme stocks are company shares with large communities of online and social media followers. Online posts about these stocks can drive significant peaks and crash their share prices [Weforum](https://www.weforum.org/agenda/2022/09/what-are-meme-stocks-explainer/#:~:text=to%20the%20article-,Meme%20stocks%20are%20company%20shares%20with%20large%20communities%20of%20online,Beyond%20and%20cinema%20chain%20AMC.). 

My three stocks are, therefore: 

- Bed Bath & Beyond (BBBY) #meme_stock
- GameStop (GME) #meme_stockre
. Nvidia (NVDA) 

To compare the evolution of their prices and to see if they have had a divergent evolution compared to the market in general. Since they are US stocks, I naturally benchmarked them against the two leading indices in the US, the S&P 500 and the Nasdaq composite.

## Result for BBBY
- Date: 09/01/2022 
- Market sentiment bearish
- Price evolution rebased on 100: down to 70 after a month 
- Price evolution of the S&P rebased on 100: down to 92 during the same time 
- Price evolution of the NASDAQ rebased on 100: down to 90 during the same period 

Comment: Here, the strategy does work and leads to more significant gain (if we short the stock)

## Result for GME 
- Date: 06/01/2022 
- Market sentiment bullish
- Price evolution rebased on 100: up to 110 after one day and stayed at this level for a few days before going back to 100 after a month 
- Price evolution of the S&P rebased on 100: on a downward path before falling to 90 
- Price evolution of the NASDAQ rebased on 100:  on a downward path before falling to 90 

Comment: Here, the strategy does work in the concise term as the stock went up during a short period before falling back again


## Result for NVDA 
- Date: 06/01/2022 
- Market sentiment bearish
- Price evolution rebased on 100: down to 88 after a month
- Price evolution of the S&P rebased on 100: down to 92 during the same period  
- Price evolution of the NASDAQ rebased on 100: down to 90 during the same time

Comment: The price evolution path here is very close to one of the two leading indices

## Conclusion
Based on the three random examples I did, it seems that out of the 3, two worked out well. However, a complete picture of data for a whole year should be observed. In addition, it turns out that the two stocks that worked well were meme stocks, as defined above.  
