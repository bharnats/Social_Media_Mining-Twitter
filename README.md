# Social Analytics-Twitter

# Observable Trends based On the data (Nov'2017)

* CBSNews and CNN express negative sentiment in their recent 100 tweets and The New York Times expresses a close neutral sentiment possible.
* Fox and BBCWorld express positive sentiment in their recent 100 tweets.
* Fox news channel expresses that all is well in United States and BBCWorld reflects the overall growth and progression of the entire world.
 
 # Background 
 __Twitter__ has become a wildly sprawling jungle of information  Somewhere between 350 million and 500 million tweets are estimated to be sent out _per day_. With such an explosion of data, on Twitter and elsewhere, it becomes more important than ever to tame it in some way, to concisely capture the essence of the data.
 
# Objective
Create a Python script to perform a sentiment analysis of the Twitter activity of various news oulets, and to present the findings visually.
The python code generated is meant to provide a cursory look at the world mood according to the Twitter profiles of news agencies. In essence, the script allows one to quickly perform a sentiment analysis on the most recent tweets of any given Twitter accounts and plot the results.The final output provides a visualized summary of the sentiments expressed in Tweets sent out by the following news organizations: __BBC, CBS, CNN, Fox, and New York times__.

# Notable libraries used to complete this application:
Matplotlib
Pandas
Tweepy
VADER Sentiment Analysis
Seaborn

# The first plot features the following: ### 
[Media_tweets](Media_Tweets.png)

* A scatter plot of sentiments of the last __100__ tweets sent out by each news organization, ranging from -1.0 to 1.0, where a score of 0 expresses a neutral sentiment, -1 the most negative sentiment possible, and +1 the most positive sentiment possible.
* Each plot point reflects the _compound_ sentiment of a tweet.
* Each plot point is sorted by its relative timestamp.

# The second plot 
[Media_Sentiments](Media_Sentiments.png)
* A bar plot visualizing the _overall_ sentiments of the last 100 tweets from each organization. 
* For this plot,the compound sentiments analyzed by VADER are aggregated.

# The final Jupyter notebook contains the following:
[Twitter_Analysis](twitter_analysis.ipynb)

* Pull last 100 tweets from each outlet.
* Perform a sentiment analysis with the compound, positive, neutral, and negative scoring for each tweet.
* Pull into a DataFrame the tweet's source acount, its text, its date, and its compound, positive, neutral, and negative sentiment scores.
* Export the data in the DataFrame into a CSV file[Twitter_Data](Twitter_Data)
* Save PNG images for each plot.

