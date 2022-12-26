# Analysis of Hotel Customer Sentiments

- Sentiment analysis is part of the Natural Language Processing (NLP) techniques that consists in extracting emotions related to some raw texts. This is usually used on social media posts and customer reviews in order to automatically understand if some users are positive or negative and why. The goal of this study is to show how sentiment analysis can be performed using python. Here are some of the main libraries we will use:

  - NLTK: the most famous python module for NLP techniques
  - Gensim: a topic-modeling and vector space modeling toolkit
  - Scikit-learn: the most used python machine-learning library

- We will use here some hotel review data. Each observation consists of one customer review for one hotel. Each customer review is composed of textual feedback of the customer's experience at the hotel and an overall rating. 
  - DataSet here: https://www.kaggle.com/jiashenliu/515k-hotel-reviews-data-in-europe

- For each textual review, we want to predict if it corresponds to a good review (the customer is happy) or to a bad one (the customer is not satisfied). The review's overall ratings can range from 2.5/10 to 10/10. 
  - In order to simplify the problem we will split those into two categories:

    - bad reviews have overall ratings < 5
    - good reviews have overall ratings >= 5

- The challenge here is to be able to predict this information using only the raw textual data from the review.
