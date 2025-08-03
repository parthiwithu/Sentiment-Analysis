# Amazon Product Review Sentiment Analysis
This project is focused on building a binary sentiment classification model using Amazon product reviews. It uses natural language processing (NLP) techniques along with a Bidirectional LSTM deep learning model to predict whether a review is positive or negative.

## Project Overview
Objective: Predict sentiment from Amazon product reviews (positive or negative).

Technologies used: Python, TensorFlow, Keras, NLTK, Scikit-learn, Pandas.

Model: Logtistic Regression, SVM, RandomForest Classifier,Naive Bayes Bidirectional LSTM.

Data source: Kaggle – Amazon Product Reviews dataset.

## Dataset
The dataset contains Amazon product reviews. A subset of 200,000 reviews is used for training. Only two columns are used:

Text: the review content.

Score: the rating provided by the user.

The score is converted to binary sentiment:

4 and 5 are labeled as positive.

1 and 2 are labeled as negative.

Reviews with a score of 3 are removed as they are considered neutral.

## Workflow
Data Cleaning and Preprocessing

Removed HTML tags and punctuation.

Lowercased all text.

Removed stopwords (with exceptions for negations).

Tokenized and lemmatized text.

Converted cleaned tokens back to string.

Tokenization and Padding

Used Keras Tokenizer to convert text into sequences.

Applied padding to make sequences of equal length.

## Model Building

Used Keras Sequential API to build a Bidirectional LSTM model.

Architecture includes an Embedding layer, Bidirectional LSTM, and Dense layers.

Used dropout to prevent overfitting.

## Evaluation

Model was evaluated using accuracy, confusion matrix, and classification report.

Training and validation loss/accuracy were visualized.

## Results
The Bidirectional LSTM model performed well in classifying review sentiment.

Demonstrated good understanding of text context and polarity.
