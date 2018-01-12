# Sentiment-Analysis-in-R
Sentiment Analysis on American Healthcare using Twitter Data.

## Data Collection

Data is collected through twitter API. As Twitter allows the users to extract only the
last one week data, it helped in getting the current emotions of the people.


## Data Cleaning

As the tweets extracted as very unstructured, it was great deal to clean the data to
extract only the sensible data for the sentiment analysis. Below is the process followed to clean the data.

• Removing all the special characters from the tweets

• Removing the usernames and hyperlinks

• Creating the corpus of text using all the tweets

• Removing stop words, punctuation, numbers, white spaces and other specific words

• Transforming the tweets to lower case


## Data Analysis

I have used lexicons from tidy text package to get the sentiments of the words. There are three types of lexicons based on the Unigram,

• AFINN from Finn Årup Nielsen,
• bing from Bing Liu and collaborators, and
• nrc from Saif Mohammad and Peter Turney

These lexicons contain many English words and the words are assigned scores for
positive/negative sentiment, and also possibly emotions like joy, anger, sadness, and so
forth. The nrc lexicon categorizes words in a binary fashion (“yes”/ “no”) into categories of
positive, negative, anger, anticipation, disgust, fear, joy, sadness, surprise, and trust.
The bing lexicon categorizes words in a binary fashion into positive and negative categories.
The AFINN lexicon assigns words with a score that runs between -5 and 5, with negative
scores indicating negative sentiment and positive scores indicating positive sentiment.
I have used ‘nrc’ lexicons to get the number of words with the different emotions.


Once the scores are assigned to the words I have grouped based on the tweet
ID and took a sum of score which gave the total sentiment of the tweet.
