# Twitter_Scraping_and_Saving

When most (non programming) people think of a tweet, it's a single social media post that consists of a 280 character message.

I was recently asked to help scrape some tweets for a professor. They provided me with three hashtags and a date range they were interested in. I asked them, "what variables are you interested in and what format would you like the data".

They responded, "Just all of the twitter data for up to 60,000 tweets in a csv file".

What this professor (and probably most people that have never munged through a tweet before) didn't realize is that it is not uncommon for a single tweet to have 360+ nested key, value pairs!

Add some additional hashtags, mentions, retweets - you can easily surpase 400 nested key, value pairs!

Tweet json returns using tweepy include the tweet text, but it also includes a ridiculous amount of information you would probably never even care about; i.e. the user's account profile_link_color.

If you've never looked at what a single tweet response looks like, I would encourage you to look at the twitter_variables_blank_example.json file in this repo.

## What's in this repo?
There are two jupyter notebook files intended to help you quickly scrape and munge tweets using python and tweepy.
Once you have your own twitter API keys, these two notebooks should enable you to scrape, munge, and save 50,000+ tweets in a csv in 30 minutes or less!

#### Tweet_Scraping_Public.ipynb
 - You need to add your own twitter API keys, look below for some info on how to get your own keys.
 - Enter a search term (#ILovePython)
 - Scrape up to 5,000 tweets at a time starting with the most recent tweet ID matching the search term
 - Adjust the tweet ID so you can search for older tweets
 - Save the tweet returns in JSON and CSV files
 - Simple Vader Sentiment Analysis
 
 #### Twitter_Munging_csv_Conversion.ipynb
 - Load and merge json files
 - Extract only the key, value pairs you are interested in
 - Save the data as json or csv files
 - Convert complete tweet json files into flattened or partially flattened csv files
 
 ## Twitter API Keys?
 
 ![]
 
 
 
 
 
