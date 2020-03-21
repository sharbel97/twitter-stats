# twitter-stats

A project initialized for myself, to later explore and create a web app in which users can access for free and obtain various data for research or recreational purposes.

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install pip.

```bash
pip3 install tweepy
```

## Usage

Here I use the method cursor() which returns an object that you can iterate or loop over to access the data collected. Each item in the iterator has various attributes that you can access to get information about each tweet including:
* The text of the tweet.
* Who sent the tweet.
* The date of the tweet was sent. 
and more.* [source](https://www.earthdatascience.org/courses/earth-analytics-python/using-apis-natural-language-processing-twitter/get-and-use-twitter-data-in-python/)

```python
import Tweepy

#Collect Tweets
text_query = 'any word or sentence'
date_since = '2019-03-20'
until_date = '2019-03-19'
tweets = tweepy.Cursor(api.search,
              q=text_query,
              lang="en",
              since=date_since).items(3) #You can add a maximum number of tweets here.
#Iterate and print tweets
for tweet in tweets:
    print(tweet.text)
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## Author

* **Sharbel Homa** 
