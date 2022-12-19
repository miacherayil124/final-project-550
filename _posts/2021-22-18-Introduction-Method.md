---
title: "Introduction & Context"
date: 2022-12-18
published: true

excerpt: "The following provides both an introduction and a brief context on the current state of EVs in the U.S. and California over the lasst decade."
toc: false
toc_sticky: false
---






This project begins by exploring twitter data and extracting a sentiment analysis from tweets between the years of 2015-2019. By using an Academic Developer API (thanks Professor Nick), we were able to scrap nearly 500, 000 tweets. We used our API tokens to initialize  several queries and used search terms like “electric vehicles, Evs, or tesla” along with the hashtags, then filtered by elimiating retweets, and tweets that contained URLs through the library Tweepy. 
As mentioned previously we filtered by start times and end times in order to control the date range of the information returned. We chose that date range due EVs increased media and public attention along with benchmarking policies like California’s 2015 Clean Energy & Reduction act, or the recent federal Infrastructure Investment and Jobs Act of 2021. 
Using the count word frequencies function we then were able to extract the top 10 word frequencies across all tweets and created a dataframe to better organize and filter our data.
 

