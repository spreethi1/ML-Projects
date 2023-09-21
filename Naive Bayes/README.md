# Spam Filtering Using Naive Bayes

## Introduction

This project, titled 'Spam Filtering Using Naive Bayes,' explores the application of the Naive Bayes algorithm for SMS spam classification. I implemented the Naive Bayes algorithm in two distinct ways to demonstrate its versatility and effectiveness. In the first approach, I built the Naive Bayes classifier from scratch, calculating probabilities and making predictions step by step. In the second approach, I utilized a pre-existing classifier model available in a popular machine learning library.

## Data

- **Dataset Source:** The SMS Spam Collection is a public set of SMS labeled messages that have been collected for mobile phone spam research. Here is the link for the dataset for your reference- https://archive.ics.uci.edu/dataset/228/sms+spam+collection
- **Dataset Size:** The dataset consists of 5572 rows and 2 columns, with 'label' indicating whether a message is spam or ham, and 'sms' containing the message text.
- **Preprocessing:**
  - There were no missing or null data points in the dataset.
  - The dataset was split into an 80-20 ratio for training and testing purposes.
  - Data cleaning involved the following steps:
    1. Removal of punctuation marks (e.g., ., !, ?) to ensure consistent text formatting.
    2. Conversion of all text to lowercase to standardize the text and avoid case sensitivity issues.
    3. Calculation of word frequencies for each term, which was necessary for building the Naive Bayes classifier from scratch.

## Methodology

The Naive Bayes algorithm, a probabilistic classification method, was employed in this project. It operates on the concept of conditional probability, making predictions based on the probability of an event given certain conditions. Specifically, we applied Naive Bayes to classify SMS messages as either spam or ham.

The implementation involved calculating the conditional probabilities of words appearing in spam and ham messages.

## Features and Feature Engineering

The features used for this SMS spam classification project are the words present in SMS messages. Each word serves as a feature. Feature engineering steps included text cleaning, removal of punctuation marks, and converting all text to lowercase to ensure consistent and standardized features.

## Model Evaluation

To evaluate the performance of our Naive Bayes spam classifier, we calculated the accuracy metric.

- Accuracy measures the proportion of correctly classified messages out of the total.
- Our model achieved an accuracy of approximately 97.94%, with 1092 correctly classified messages and 23 incorrectly classified messages.
