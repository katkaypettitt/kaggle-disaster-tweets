# Natural Language Processing with Disaster Tweets

> My entry for the [Disaster Tweets Kaggle competition](https://www.kaggle.com/c/nlp-getting-started/) which received a public score of 0.78945 and was submitted in March 2021. Competition participants create a machine learning model to detect which tweets are about real disasters and which ones aren't.  



## General info

Both the train and test datasets were manually cleaned using pandas and regular expressions, including expanding contractions and removing accents, special characters, and stopwords. A variety of features were then extracted to find, for example, the amount of hashtags, urls, word tokens, and tweet tokens for each entry. 

After visualising and observing the engineered features, they were prepared for model training. This involved utilising a TFID Vectoriser and fitting the cleaned dataset with the selected features via a sparse matrix. In the end, four features were transformed and fit to the cleaned dataset. 

Three different models, a Naive Bayes classifier, logistic regression, and support vector classifier, were trained and optimised according to their F-scores. The logistic regression model was found to be the best fit for the data.

The following files are included in this repo:

* `disaster_tweets.ipynb`: the code
* `disaster_tweets_submission.csv`: predictions for test dataset
* `train.csv`: train dataset
* `test.csv`: test dataset



## Technologies

Python 3.7.6
