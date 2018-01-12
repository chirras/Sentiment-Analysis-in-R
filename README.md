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


