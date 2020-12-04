## Emoci : Emoji Prediction from Tweets (CS-464 Course Project)

### Group Members
Adil Meriç            21802660  
Alperen Öziş             21703804  
Arda Göktoğan            21702666  
Onur Oruç            21702381  
Osman Batur İnce        21802609  

### Description of the Data

As Twitter has a user database that uses emojis and allows users to express their thoughts only on 140 characters, we have looked up for tweet databases. We have found that EmojifyData dataset offers 18 million unique tweets with emoji(s) included. In addition, the dataset is based on ArchiveTeam Twitter Stream, which is a part of Archive.org. However, as the dataset’s tweets are heavily random, we will have to make preprocessing. We will eliminate the tweets according to some metrics (e.g. containing profanity, more than one emoji type). To simplify the data, we will select tweets with the most used 15-25 emojis and give a label to each of them. To store the data, we will form a data file where we store the tweet id in the first column, texts in the tweets in the second column, and the emoji label according to the text in the third column.

### Precise Description of the question you are trying to answer with the data

data
We will try to find the relation between sentence and emojis. Given a text of a tweet, we will try to predict which emojis might have been used in that tweet. First, we will train a dataset of sentences with emoji labels to build a classifier that pairs emojis with sentences. Then the classifier we built will take a sentence as an input and will output the most probable emoji to be used in that sentence.

### What you plan to achieve by the milestone

In this project we plan to use different word embedding methods and different algorithms. The word embedding methods we are planning to use can be listed as ELMo, Word2Vec, Glove. As a starting point, we plan to use the multinomial naive bayes classifier with the bag of words (BoW) method. Then we plan to use SVM and LSTM with different word embedding methods which are previously stated. Until the first demo, we plan to implement and test multinomial naive bayes and SVM with different word embeddings. After the first demo, we plan to enhance our work with LSTM and pre-trained models such as Bert or XLNet. At the end of the final report and analysis according to the algorithms and word-embedding methods, we plan to create an interactive application to use our prediction algorithms.
