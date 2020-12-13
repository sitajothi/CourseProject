# Overview of our Stock Sentiment Analyzer

Our project aims to analyze stock sentiment from Twitter data to help our users understand whether or not to buy or sell stocks. Understanding sentiment from tweets is very helpful as it provides textual context to the market outlook of different stocks.

We started by running a pre-existing sentiment analyzer, Vader, to have a baseline performance. Then, we did research into different methods of sentiment analysis to build our own sentiment analyzer, which we trained on a kaggle dataset, and later tested on the Twitter API using recent tweets. We wanted our user to easily understand the sentiment of a stock’s set of tweets, so we added a pie graph as a visualization for user’s to make the stock purchasing decisions.

# Stock Sentiment Analyzer Setup and Usage

Firstly, the user must have access to Jupyter notebook. There is a browser version, which the user can find with a google search for “Jupyter notebook browser.”

Our application also uses the Twitter API. To be able to receive real time information, the user must create a developer portal on Twitter and gain Access Tokens and Keys. Additionally, the user must save their credentials in a json format to a file called: twitter_credentials.json so that the application can pull them. (e.g. {"CONSUMER_KEY": "", "CONSUMER_SECRET": "", "ACCESS_TOKEN": "", "ACCESS_SECRET": ""})

Once these two steps are complete, the user can proceed to the last cell of the Jupyter notebook to change the ticker name. The ticker name must be in a string format with a preceding ‘$’. To run our application, the user can click on Cell -> Run All, and they will see a pie graph with the sentiment distribution corresponding to that stock.
