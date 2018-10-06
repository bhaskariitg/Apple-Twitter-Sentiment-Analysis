# Apple Twitter Sentiment Analysis
Here we have got a dataset in which one of our predictor is in form of text(The Tweets).

Now Tweets are:

1. Loosely Structured

2. Textual

3. Poor Spelling, non-traditional grammer

4. Can be Multilingual

The goal here is to understand and derive meaning from human language.

The dataset which was provided to us contains tweets from the user along with the sentiment and somme other variables like Unit_id, date etc. Now the sentiment of the tweets are divided into 4 categories. In sentiment column if we see:

1 -> it means that the tweet is of negative sentiment

3 -> it means that the tweet is of neutral

5 -> it means that the tweet is of positive sentiment

and the tweets sentiment also contains one more entry named not_relevant which means that the tweet does not show any sentiment towards Apple.

Now using the tweets as predictor we have to predict the sentiment. We have to correctly classify tweets as being positive, negative, neutral and not relevant. To do that we will use Bag of words approach, and build our text analytics model.

Here we know that the tweets are an important independent variable as the tweets contain certain words which we can label as being good or bad about Apple. Here our model will just count the no of times each word appears in the text and use these counts as the independent variable. For preprocessing the data we have to:

1. Change all the words to either lower or upper case.

2. Remove punctuation.

3. Remove stopwords as they are not likely to improve the machine learning prediction.

4. Stem the Words.

Packages Used:

1. CaTools - To seperate our dataset into 2 subsets named Train and Test set.

2. tm and SnowballC - tm is the text mining package and SnowballC package lets us use the tm package.

3. Random Forest - To build a model based on the concepts of Random Forest.

4. e1071 - Build a support vector machines model.

Now after we have built our model, use the test set to check the accuracy of our model.

The accuracy which we get from

Random Forest is: 68.295%

SVM is: 69.237%

The accuracy of both is more than our Baseline model.

When we apply cross validation, accuracy increased slightly then what was without cross validation.

