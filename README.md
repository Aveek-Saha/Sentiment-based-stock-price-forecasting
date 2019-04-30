# Apple Stock Price Forecasting using Sentiment Analysis

Using the [sentiment140 dataset](http://help.sentiment140.com/for-students/) we trained 4 models for binary sentiment classification. The models are- 
* SVM
* Logistic regression
* Naive Bayes
* LSTM

The historical Apple stock prices(AAPL) were downloaded from Yahoo finance for the period 01-02-2008 to 01-02-2019. Then Tweets and NY Times news articles were collected from the same time period about Apple and some Apple products like Macbooks, iPhones etc. Using the best of the 4 models trained above, the Tweets or News articles were classified as having positive or negative sentiment, then an overall sentiment value is assigned for each day. 

Now with the opening stock price and a sentiment score, an LSTM with a 60 day window is used to predict future stock prices.

## Order of execution- 
1. Preprocess_datasets.ipynb
2. Train_sentiment_model.ipynb
3. Create_stock+sentiment_datasets.ipynb
4. Stock_prediction_LSTM.ipynb

