# Twitter Airline Reviews Sentiment Analysis

### INTRODUCTION : 

Social Media has taken the world by surprise at a swift and commendable pace. With the advent of any kind of circumstances may it be related to social, political or current affairs the sentiments of people throughout the world are expressed through their help, making them suitable candidates for sentiment mining. Sentimental analysis becomes highly resourceful for any organization who wants to analyse and enhance their products and services.

The feedback/ reviews of some of the airlines are collected from tweets of the users on Twitter, for conducting a sentiment analysis on their respective customers.
The tweets are extracted and pre-processed and categorized the sentiments of the tweets as positive, negative and neutral.
### About the dataset :-

This sentiment analysis dataset contains tweets since Feb 2015 about each of the major US airline. Each tweet is classified either positive, negative or neutral.
The data can be loaded from the following link : https://www.kaggle.com/crowdflower/twitter-airline-sentiment
The dataset originally consists of 15 columns. These are :
1. tweet_id
2. airline_sentiment
3. airline_sentiment_confidence  
4. negativereason                  
5. negativereason_confidence        
6. airline                            
7. airline_sentiment_gold          
8. name                                
9. negativereason_gold             
10. retweet_count                     
11. text                                
12. tweet_coord                     
13. tweet_created                      
14. tweet_location                   
15. user_timezone


Sentiment analysis is performed on the dataset to predict the sentiments of the reviews - positive or negative.

You can view the notebooks uploaded in the same repository in the given order: 
1. [Twitter airline sentiment analysis - Visualisation](https://colab.research.google.com/drive/18h85gbCA87ZIfnVTD_ax9TAglGKn0slg?usp=sharing)
2. [Twitter airline sentiment analysis - Model Training 1](https://colab.research.google.com/drive/15_5z-ak0sYNAoD0alqpjzgpIMDCHP55k?usp=sharing)
3. [Twitter airline sentiment analysis - Model Training 2](https://colab.research.google.com/drive/1SIirL8HeS4HCCmNBREof3nX1D9kzGM9R?usp=sharing)


### Results : 
I have trained the dataset using WordEmbedding for Neural Networks, using CountVectorizer() for Logistic Regression, KNN and Naive Bayes and using TfidfVectorizer() for Neural Networks in three separate notebooks respectively.

##### Accuracies of models trained with the mentioned classifiers -
  * Using Word Embeddings for Neural Networks 
     | Training accuracy  | Validation accuracy |
     | -----------------  | ------------------- |
     |     86.98%         |     83.95%          |
     
  * Using CountVectorizer()
     |   Classifiers       |   Accuracy           | 
     | -----------------   |   -----------------  | 
     | Logistic Regression |       83.07%         | 
     |  KNN                |       64.09%         | 
     | Naive Bayes         |       59.85%         |   
  
  * Using TfidfVectorizer() for Neural Networks: 
     | Training accuracy  | Validation accuracy |
     | -----------------  | ------------------- |
     |     76.95%         |     76.29%          |


### Conclusion:-
1. It is observed that NeuralNetworks using Word Embeddings performs better than by using tfidfVectorizer() for the same.
2. Logistic Regression model using CountVectorizer() has a better accuracy than the other classifiers.
3. Training the model by vectorizing the texts using CountVectorizer() performs better than using TfidfVectorizer().
