# Twitter_Scraping_and_Saving

This repo has two jupyter notebooks designed to make it easy to scrape, munge, and save tweet data in csv or json files.

## What kind of data do you want to scrape?

When most (non programming) people think of a tweet, it's a single social media post that consists of a 280 character message.

I was recently asked to help scrape some tweets for a professor. They provided me with three hashtags and a date range they were interested in. I asked them, <i>"what variables are you interested in and what format would you like the data".</i>

They responded, <i>"Just all of the twitter data for up to 60,000 tweets in a csv file".</i>

What this professor (and probably most people that have never munged through a tweet before) didn't realize is that it is not uncommon for a single tweet to have <b>300+ nested key, value pairs!</b>

Add some additional hashtags, mentions, retweets - you can easily surpase 400 nested key, value pairs!

Tweet json returns using tweepy include the tweet text, but it also includes a ridiculous amount of information you would probably never even care about; i.e. the user's account profile_link_color.

If you've never looked at what a single tweet response looks like, I would encourage you to look at the twitter_variables_blank_example.json file in this repo. This example has more than 360 key, value pairs from a single tweet!

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

<p align="center">
<img src="img/tweet_scraping_code_example.png" width="600" height="545" title="screenshot">
</p>

#### Twitter_Munging_csv_Conversion.ipynb
 - Load and merge json files
 - Extract only the key, value pairs you are interested in
 - Save the data as json or csv files
 - Convert complete tweet json files into flattened or partially flattened csv files

<p align="center">
<img src="img/tweet_sorting_code_example.png" width="800" height="539" title="screenshot">
</p>

## Twitter API Keys?
 
 I used a python library <a href="https://github.com/tweepy/tweepy">Tweepy</a> to access Twitter's API to scrape data.
 You will need to enter your own twitter API keys for tweepy to authenticate properly.
 
 <p align="center">
<img src="img/twitter_keys.png" width="600" height="227" title="screenshot">
</p>
 
 <b>Warning</b> Generating Twitter API keys isn't a simple 5 minute process. It can take anywhere from minutes to weeks to get a Twitter Developer account approved so you can generate API keys - so have some patience and plan ahead!
 
To create a Twitter Developer account, visit <a href="https://developer.twitter.com/en/apply-for-access.html">Twitter Developer</a> and apply for access. 


 
 
