# IMDb Movie Review Sentiment Analysis

## Introduction
This project aimed to predict the sentiment of IMDb movie reviews as either positive or negative using natural language processing and machine learning techniques. The dataset consists of 50,000 IMDb movie reviews from Stanford University, divided into training and testing sets.

## Data Loading
The IMDb movie reviews were loaded into Pandas data frames from .txt files, with labels (1 for positive, 0 for negative) added. Both the training and test sets contain 25,000 reviews each, evenly split between positive and negative sentiments.

## Data Preprocessing
Data preprocessing involved several steps, including tokenization, stop word removal, lemmatization, removing special characters and punctuation, and converting all words to lowercase. The preprocessed data was stored in the review column.

## Vectorization
Vectorization using Bag of Words transformed the text data into numerical features, which are essential for machine learning. The resulting data frames had 25,000 rows and 63,875 columns, each representing a word's presence and frequency.

## Data Split
The training set consisted of 25,000 reviews for model training, while the testing set was used for validation and testing. A 70/30 split was maintained to avoid data mixing.

## Model Type and Architecture
A neural network model was used to predict sentiment. It consisted of multiple layers and neurons, with ReLU activation functions and dropout applied to prevent overfitting. The architecture was chosen to effectively capture complex features for sentiment prediction.

## Results
The model achieved a training accuracy of 89.55% and a validation accuracy of [Provide Validation Accuracy Here]. For Model 2: Predicting Crime Count, the Mean Squared Error (MSE) on the test set was 233.25, indicating a well-fitted model. The results showed that the neural network outperformed previous models in sentiment analysis and crime count prediction.

## Data Source
- [Stanford 50,000 IMDb Movie Reviews Dataset](http://ai.stanford.edu/~amaas/data/sentiment/)
  - [Train Data](http://ai.stanford.edu/~amaas/data/sentiment/aclImdb_v1.tar.gz)
  - [Test Data](http://ai.stanford.edu/~amaas/data/sentiment/aclImdb_v1.tar.gz)
