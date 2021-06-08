# Twitter Machine Learning
#### Mala Sharma, George Mihalopoulos, Alex Narvaez-Duckworth

## Project Scope: 
Today, the world is more connected than we have ever been in history. A single Tweet from one individual can potentially create market reactions. Most recently, we've seen influencers like Elon Musk contribute to this narrative in regards to Bitcoin's price action, especially surrounding the announcement that Tesla would not be accepting bitcoin as payment for Tesla vehicles. This idea was the foundation of our research where we applied Natural Language Processing to a selection of web-scraped Tweets. These tweets were from influencers in the cryptocurrency space such as Elon Musk, Charles Hoskinson, Michael Saylor and even Dave Portnoy. Our intention was to extract an NLP analysis from these users to understand what their sentiment was like year to date, and whether or not that had any correlation to the cryptocurrency market. 

## Question 1 
#### Why did we choose to only analyze the Twitter accounts of influencers from the cryptocurrency sphere? Why didn't we analyze subreddits and niche Facebook posts? 
We decided to analyze Twitter for several reasons. The first being that Twitter has grown exponentially in popularity amoung Milenials and Generation Z, but also with older generations who have arguably access to more capital for investment. These Twitter accounts reach a higher amount of individuals within that demographic. Additionally, Tweets are easily tracable, providing us with ample data to run our analysis. The Twitter content that goes viral, such as Elon Musk's content, often makes it to these other more niche social platforms, sometimes in more diluted meme form. Thus, we would consider Twitter to be our "primary source" material for research.

## Question 2 
#### Why did we decide to perform analysis on Bitcoin closing prices and not any other coins (i.e. dogecoin & ethereum)?
Bitcoin is a major currency in the crypto market that has the most prevalence outside of the estoteric cryptosphere with widely recognizable supporters such as Elon Musk and Miami mayor Francis Suarez proposing to pay workers in Bitcoin. More recently, El Salvador President Nayib Bukele has offered Bitcoin as official legal tender, especially for El Salvadorian ex-patriots to send money home in the form of decentralized remittances. Bitcoin is also considered the largest token by market cap in the cryptocurrency market. Within the short time-frame of this project, we did not find price feeds for the total market caps of the entire cryptocurrency market. Thus Bitcoin currency serves as metonymy for the cryptocurrency market.

## Question 3
#### Which Twitter-based cryptocurrency influencers did we choose to analyze and apply Natural Langauge Processing to?
###### mike = ('michael_saylor') Michael Saylor https://twitter.com/michael_saylor
###### elon = ('elonmusk') Elon Musk https://twitter.com/elonmusk
###### woo = tweet_sentiment('woonomic') Willy Woo https://twitter.com/woonomic
###### t360 = tweet_sentiment('360_trader')https://twitter.com/360_trader
###### whale = tweet_sentiment('CryptoWhale')https://twitter.com/ShibaInu_Rise
###### charles = tweet_sentiment('IOHK_charles')https://twitter.com/IOHK_Charles
###### mark = tweet_sentiment('mcuban') Mark Cuban https://twitter.com/mcuban
###### kevin = tweet_sentiment('kevinolearytv') https://twitter.com/kevinolearytv
###### joel = tweet_sentiment('JoelKatz') https://twitter.com/JoelKatz
###### dave = tweet_sentiment('stoolpresidente')https://twitter.com/stoolpresidente

## Analysis: 
### Fear and Greed Index 
The Bitcoin Fear and Greed index is a number between 0-100 that helps indicate when investors are too fearful, or too gready. The index takes into consideration several factors. 

###### Volatility : the program marks wider fluctuations as a sign of fear
###### Market volume : When buying volumes increase significantly, the greed levels rise, too
###### Social media : Monitors, gathers and counts posts on various hashtags, to see how many interactions they receive over certain time-frames
###### Dominance : Once Bitcoin dominance rises, it indicates an increasing level of greed, and vice versa, when the dominance shrinks, it means that people get scared to invest in BTC. 
###### Trends : The program pulls Google Trends data for various Bitcoin-related search queries and crunches those numbers, especially the change of search volumes 

Although no metric provides perfect indicators on whether to buy or sell, the Fear and Greed index can provide indicators regaurding overall market sentiment. As seen in the chart below, the fear and greed index trendline has been steadily increasing since its inception. In addition, the FNG index shows prevelent "boom and bust" cycles which can be represented in Bitcoin bull/bear markets. 
![FNG Trendline](/images/FNG%20Trendline.png)

### Bitcoin Price Movements
In the last year, there had been several major events that had impacted the crypto space significantly. Since its inception, the currency has seen rapid addoption. In August of last year, Microstrategy had been the first publically traded company to hold all of their cash reserves in Bitcoin. The decision coming from large Bitcoin supporter Michael Saylor. Since then, Bitcoin's price had increased drastically, reaching $60,000. Recently this last month, there had been several major events that had led to the crypto's fall from all-time high's. In the same time period as Coinbase's IPO, Tesla had announced that Bitcoin will not be an acceptable payment for Tesla vehicles citing the Bitcoin mining environmental concerns. The additional slip in price had been caused by China's crackdown on the crypto currency by not allowing Chinese brokers to purchase Bitcoin. 
![Bitcoin Price](/images/Bitcoin%20Price%20Chart.png)


### Bitcoin Price / FNG
Below is a chart illustrating the Bitcoin price / FNG. Large spikes within those metrics can indicate bearish patterns. Typically, large spikes like that occurs when the FNG index dips drastically showing a downtrend in not only the index, but Bitcoin price as well. In the last month, we have been in the midst of similar volitility. 
![Bitcoin/FNG](/images//Bitcoin%20Close%20:%20FNG.png)

### Bitcoin Algorithm
In our analysis of the FNG index and closing price, we had created a Deep Learning Algorithm to help potentially predict Bitcoin movements. The model takes into account two variables, the closing price and FNG index value. Although it is not as efficient in predicting exact prices, it does show potential price swings. This, coupled with the Twitter sentiment analysis below gives us a very good picture of sentiment surrounding the Crypto environment.
![Bitcoin Algorithm](/images/Algoritm%20Performance.png)

### Tweet Sentiment Bar Chart
In our analysis of web scraped tweets, it seemed best to visualize the data in a bar graph. To accomplish this we resampled all of our data to aggregate daily means of compound sentiment data (combination of positive, neutral, and negative). This way, we were able to visualize daily sentiment levels for each account on a daily basis. What we found was that among the accounts we chose, it appears that they are generally positive. These are leaders in their space and influencers on the internet so it only seems right that most of their public discourse is either positive or neutral. However, this provided a great opportunity to really distinguish individual days as having significant negative sentiment as well as increased concentrations of negative sentiment.
![Sentiment Bar Chart](/images/tweetscrape_barchart.png)

### Tweet Sentiment Box Plot
We decided to include a box plot for each user account in order to determine the range of positive to negative sentiment. As was seen in the bar chart, most users are generally positive. The accounts whose range of sentiment extends most negative are David Schwartz/Joel Katz (-0.9724), Crypto Whale (-0.9676), and Mark Cuban (-0.9231). Of all the accounts the one with the smallest box and whisker plot range and interquartile range is Dave Portnoy.
![Sentiment Box Plot](/images/tweetscrape_boxplot.png)
