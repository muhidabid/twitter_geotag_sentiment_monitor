<-------------------------------------------------------------->
Created by: Muhid Abid Siddiqui, Zoha Jaleel
Date: 26/06/2021
<-------------------------------------------------------------->


<------- Description ------->

Written in 𝗣𝘆𝘁𝗵𝗼𝗻, the model essentially fetches recent public tweets given a certain number of rules/filters, like keywords or hashtags. This is done using the Twitter API.

The tweets are received as JSON objects, including different basic metrics about the tweet. We used regex to extract the exact text of the tweet and clean it.

Once preprocessed, the sentiments of the tweets are analyzed and it is found if a tweet is a personal opinion or a factual statement. These are done using 𝗧𝗲𝘅𝘁𝗕𝗹𝗼𝗯's polarity and subjectivity properties.

The results are then stored and visualized in real-time using 𝗺𝗮𝘁𝗽𝗹𝗼𝘁𝗹𝗶𝗯 graph animation.

Unfortunately, we didn't have access to Twitter API's geotag data because we had a 'Standard Twitter Team Developer' account and not an 'Academic Research' account. So we had to improvise and assign a location to a tweet on the basis of probabilities. 

Given access to proper data with real geotags, this tool can be used to monitor public sentiments about important current topics, politics, influential people etc.

Note: Current project is tuned to monitoring political tweets in Pakistan. You can change the topic to anything you like.

<-------- HOW TO RUN -------->

1. insert your Twitter API keys in keys.py
2. run stream.ipynb
3. run visualzie.ipynb

* Note: Sentiment counts are stored in IK_tweets_provincial_stats.csv
	Latest tweet is stored in tweet.txt
