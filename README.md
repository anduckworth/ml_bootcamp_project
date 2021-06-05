# Twitter Machine Learning
#### Mala Sharma, George Mihalopoulos, Alex Narvaez-Duckworth

## Project Scope: 
Today, the world is more connected than we have ever been in history. A single Tweet from one individual can create market reactions. More recently in the last month, Elon Musk attributed to Bitcoin's fall from all-tiem high's in the last month by accouncing Tesla will not be accepting the commodity as payment for Tesla vehicles. This led us to do more reserach on the topic and apply Natural Language Processing to a selection of web-scraped Tweets. These tweets were from notable accounts in the cryptocurrency space such as Elon Musk, Charles Hoskinson, Altcoin Daily, and even Dave Portnoy. Our intention was to extract an NLP analysis from these users to understand what their sentiment was like year to date, and whether or not that had any correlation to the cryptocurrency market. Using our cryptocurrency API data, can we test and train a model that predicts actual closing prices with an accuracy close to 70%

## Question 1 
#### Why did we choose to only analyze the Twitter accounts of influencers from the cryptocurrency sphere? Why didn't we analyze subreddits and niche Facebook posts? 
We decided to analyze Twitter for several reasons. The first being that Twitter has grown exponentially in popularity amoung Milenials and Generation Z. These accounts reach a higher amount of individuals within that demographic. Additioanlly, Tweets are easily tracable, prodividing us with ample data to run our analysis. 

## Question 2 
#### Why did we decide to perform a close read of the Bitcoin closing prices and not any other coins (i.e. dogecoin & ethereum)?
Bitcoin is a major currency in the crypto market that has the most prevalence outside of the niche cryptosphere with widely recognizable supporters such as Elon Musk and Miami mayor Francis Suarez proposing to pay workers in Bitcoin. 

## Question 3
#### Which Twitter-based cryptocurrency influencers did we choose to analyze and apply Natural Langauge Processing to?
mike = ('michael_saylor') Michael Saylor https://twitter.com/michael_saylor
elon = ('elonmusk') Elon Musk https://twitter.com/elonmusk
woo = tweet_sentiment('woonomic') Willy Woo https://twitter.com/woonomic
t360 = tweet_sentiment('360_trader')https://twitter.com/360_trader
whale = tweet_sentiment('CryptoWhale')https://twitter.com/ShibaInu_Rise
charles = tweet_sentiment('IOHK_charles')https://twitter.com/IOHK_Charles
mark = tweet_sentiment('mcuban') Mark Cuban https://twitter.com/mcuban
kevin = tweet_sentiment('kevinolearytv') https://twitter.com/kevinolearytv
joel = tweet_sentiment('JoelKatz') https://twitter.com/JoelKatz
dave = tweet_sentiment('stoolpresidente')https://twitter.com/stoolpresidente

## Analysis: 
#### Fear and Greed Index 
The Bitcoin Fear and Greed index is a number between 0-100 that helps indicate when investors are too fearful, or too gready. The index takes into consideration several factors. 

`Volatility : the program marks wider fluctuations as a sign of fear`
Market volume : When buying volumes increase significantly, the greed levels rise, too
Social media : Monitors, gathers and counts posts on various hashtags, to see how many interactions they receive over certain time-frames
Dominance : Once Bitcoin dominance rises, it indicates an increasing level of greed, and vice versa, when the dominance shrinks, it means that people get scared to invest in BTC. 
Trends : The program pulls Google Trends data for various Bitcoin-related search queries and crunches those numbers, especially the change of search volumes 

Although no metric is provides perfect indicators on whether to buy or sell, the Fear and Greed index can provide indicators regaurding overall market sentiment. As seen in the chart below, the fear and greed index trendline has been steadily increasing since its inception. In addition, the FNG index shows prevelent "boom and bust" cycles which can be represented in Bitcoin bull/bear markets. 
![FNG Trendline](/images/FNG%20Trendline.png)
https://github.com/anduckworth/ml_bootcamp_project/blob/main/images/FNG%20Trendline.png
![]()<br>
###
![]()<br>
###
![]()<br>
###
![]()<br>
### 
![]()<br>
###
![]()<br>
###
![]()<br>
### 
### Question 4<br>

### Response <br>
![]()<br>
### Question 5<br>


### Response <br>
![]()<br>
### Question 6<br>


### Response <br>
![]()<br>
### Question 7<br>


### Response <br>
![]()<br>
### Question 8<br>

### Response <br>
![]()<br>
