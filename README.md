# Fake_News_Detection
ML Project to classify fake and real news 
Objective:
The objective of this assignment is to develop a Semantic Classification model. You will be using Word2Vec method to extract the semantic relations from the text and develop a basic understanding of how to train supervised models to categorise text based on its meaning, rather than just syntax. You will explore how this technique is used in situations where understanding textual meaning plays a critical role in making accurate and efficient decisions.

# Business Objective

The spread of fake news has become a significant challenge in today’s digital world. With the massive volume of news articles published daily, it’s becoming harder to distinguish between credible and misleading information. This creates a need for systems that can automatically classify news articles as true or fake, helping to reduce misinformation and protect public trust.
In this assignment, you will develop a Semantic Classification model that uses the Word2Vec method to detect recurring patterns and themes in news articles. Using supervised learning models, the goal is to build a system that classifies news articles as either fake or true.

## Important Point while running the python code 

In Section 6.1 we tried directlly loading the word2vec_model from gensim api sometimes it doesnt work then follow the steps mentioned in comment and uncomment the commentted last line of code and load the word2vec from your local 

import gensim
import gensim.downloader as api
word2vec_model = api.load("word2vec-google-news-300")

'''If the loading from the internet does not work, use the below line to load it from local directory
before that download the "GoogleNews-vectors-negative300.bin" file and place it in the same directory as this notebook
use below URL to download the file
https://s3.amazonaws.com/dl4j-distribution/GoogleNews-vectors-negative300
or
https://www.kaggle.com/datasets/leadbest/googlenewsvectorsnegative300?resource=download
'''

#word2vec_model = KeyedVectors.load_word2vec_format("GoogleNews-vectors-negative300.bin", binary=True)

