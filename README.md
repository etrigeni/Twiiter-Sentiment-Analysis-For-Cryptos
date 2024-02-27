# Twiiter-Sentiment-Analysis-For-Cryptos



**Introduction**

Twitter sentiment analysis for Bitcoin BNB and Ethereum. The aim was using tweets that extracted from twitter, to examine the sentiments of people about these coins. Because of the fact that their price increases and decreases daily, we considered that may the sentiments of the people change according the cryptos’ value.


**Methodology**

We used Twitter API and in combination with Python we managed to collect 3707 tweets. Actually we collected more than these but there were a lot of duplicates that we abstracted in the sequel. The reason that we had duplicates was that the date was in a datetime format. So even we wrote a piece of code to avoid duplicates, because of the fact that every second the seconds in the date were changing, every new record was considered as unique. An other issue that caused duplicates is that every second the tweets get likes. So again, every record was considered as unique because it had a different number of likes even if it had the same text and was written by the same user.So, we removed duplicates and carried on with the 3707 unique tweets. We did data preprocessing and we removed urls, emoticons and unwanted punctuations.


Our tweets dataset is consisted of the following attributes: text, username, user description, number of user’s followers, likes, number of user’s tweets, number of account’s retweets, date that tweet was created, location, hashtags, sentiment and subjectivity. Subjectivity indicates if a tweet is a personal opinion so in this case the tweet is considered as subjective, or it refers in factual information, so the tweet is considered as objective.


Using TextBlob we classified the tweets according to the sentiment as negative, positive or neutral and according to the subjectivity as objective, subjective or neutral. Also we used Matplotlib and Seaborn frameworks in order to create our plots.
In our MySQL database are stored 6838 tweets but we used only the unique 3707 tweets for the analysis. So all the below findings are based on these 3707 tweets. 


From them, 1762 have the hashtag Bitcoin,1452 have the hashtag Ethereum and 1073 have the hashtag BNB. Bitcoin is the most popular cryptocurrency and that’s why more tweets contain this hashtag as we will see in the sequence.
We collected these tweets in a period of 4 days (23/02/2022-26/02/22). In the next section we will present our findings.
