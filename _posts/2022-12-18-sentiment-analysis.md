---
title: "Sentiment Analysis from Twitter Data"
date: 2022-12-18
published: true

excerpt: "Understanding trends in the sentiments around electric vehicles between 2015 and 2019"
toc: false
toc_sticky: false
---
This project begins by exploring twitter data and extracting a sentiment analysis from tweets between the years of 2015-2019. 
By using an Academic Developer API (thanks Professor Nick), we were able to scrap nearly 33,000 tweets. We used our API tokens to initialize  several queries and used search terms like “electric vehicles, Evs, or tesla” along with the hashtags, then filtered by eliminating retweets, and tweets that contained URLs through the library Tweepy. 
 

## Top 10 most common words gathered from tweets related to electric vehicles
Using the count word frequencies function we then were able to extract the top 10 word frequencies across all tweets and created a dataframe to better organize and filter our data.


![Fig1]({{ site.url }}{{ site.baseurl }}/assets/images/Fig1.png)

## Top 10 most common words without stop words
Using the count word frequencies function we then were able to extract the top 10 word frequencies across all tweets and created a dataframe to better organize and filter our data. We filtered by start and ed times, eliminated urls and common stop words. Expectantly, car and tesla were the most frequent words. 

![Fig2]({{ site.url }}{{ site.baseurl }}/assets/images/Fig2.png)

## Top 10 most common words without search key words
When eliminating our search words, the following figure displays the the top words in query. 


![Fig3]({{ site.url }}{{ site.baseurl }}/assets/images/Fig3.png)

## Measuring polarity
Once we filtered for our target words, start and end times, eliminated urls and common stop words, we were able to perform a sentiment analysis using the textbob . We then created a number of fields and a dataframe inlcusing date, text, polarity and subjectivity. The median polarity of tweets is 0.16, the mean 0.17. This indicates a slightly positive skew to the discussion surrounding electric vehicles.T

![Fig4]({{ site.url }}{{ site.baseurl }}/assets/images/Fig4.png)

## Measuring subjectivity
The median subjectivity is .5 (on a scale of zero to one) indicating that the subjectivity skews lower.
![Fig5]({{ site.url }}{{ site.baseurl }}/assets/images/Fig5.png)

## Overall nature of tweets
We then plot subjectivity and polarity against each other, and observe the trend that as subjectivity increases, so does polarity in both directions. That is, as the tweets get more and more subjective, they are also either most positive or more negative.


![Fig6]({{ site.url }}{{ site.baseurl }}/assets/images/Fig6.png)

![Fig7]({{ site.url }}{{ site.baseurl }}/assets/images/Fig7.png)

## Trends in polarity and subjectivity through the years
When grouping the biased tweets by the year we were able to generate two box and whiskers plots of polarity and subjectivity for each year between 2015-2019. Polarity is mostly positive but has been on a steady decline since 2015. The last plot tells a similar story and skewing more negative the close to 2019. 



![Fig8]({{ site.url }}{{ site.baseurl }}/assets/images/Fig8.png)

![Fig9]({{ site.url }}{{ site.baseurl }}/assets/images/Fig9.png)


It seems that EV sentiments are more nuanced than we initially thought and will seemingly to continue to evoke varied responses. We recongize that scrapping  twitter data only provides us with a narrow perspective of EVs, and perhaps a classic community survey would do a much better job of capturing a more diverse sample size. 
As hybrid and electric vehicles  slowly become more affordable to the general public, other opinions based on equity, affordability, and EV charging stations will continue to  be at the forefront of the EV conversation both on and off twitter. 
