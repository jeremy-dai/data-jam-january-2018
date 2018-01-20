# data-jam-january-2018

Since it's been freezing in houston recently, we thought it might be fun to have a dataset that takes stock of Houston's current mood. We pulled in data using twitter's api following the #houwx hashtag. [Justin Gosses](https://twitter.com/JustinGosses) pulled the dataset, and [Yulan Lin](https://twitter.com/y3l2n) worked on munging it. The csv contains a lot less information than the raw json dump from the api, but is more structured.


## datasets

### houwx.csv
fields

- text: text of the tweet, potentially truncated
- id: id of the tweet
- favorite_count: number of favorites
- is_quote_status: if it was a quote
- retweet_count: how many retweets
- username: screen name of the user
- followers: number of followers of the user
- verified: whether or not the user is verified
- description: user's description in their profile
- user_location: user_location
- create_at: timestamp

### houwx.json
this is the raw data, which contains many more fields, but is also a lot messier

You can read more about the JSON data structure here in the [Twitter API](https://developer.twitter.com/en/docs/tweets/data-dictionary/overview/intro-to-tweet-json).
