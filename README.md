# SportVsPoliticsTextClassification

## Project Overview

This project focuses on classifying text documents into two categories:
SPORT and POLITICS. The dataset used is a subset of the 20 Newsgroups
dataset. The objective of this work is to compare different machine
learning algorithms and analyze their performance on text data.

The project applies TF-IDF feature extraction and evaluates three
models: - Multinomial Naive Bayes - Logistic Regression - Support Vector
Machine (Linear SVM)

The results are compared using accuracy and F1-score metrics.

------------------------------------------------------------------------

## Dataset Information

The 20 Newsgroups dataset contains approximately 20,000 documents across
20 different topics. For this project, the following categories were
selected:

-   rec.sport.baseball
-   rec.sport.hockey
-   talk.politics.guns
-   talk.politics.mideast
-   talk.politics.misc

The sports-related categories were merged into a single class called
SPORT, and the politics-related categories were merged into a single
class called POLITICS.

To prevent bias, metadata such as headers, footers, and quoted text was
removed before training.

------------------------------------------------------------------------

## Preprocessing and Feature Engineering

Text data was converted into numerical format using TF-IDF
vectorization. Both unigram and bigram features were used to capture
individual words and short phrases. English stopwords were removed to
reduce noise in the data.

------------------------------------------------------------------------

## Machine Learning Models Used

1.  Multinomial Naive Bayes\
2.  Logistic Regression\
3.  Support Vector Machine (Linear SVM)

Each model was trained using an 80-20 train-test split.

------------------------------------------------------------------------

## Evaluation Metrics

Model performance was evaluated using:

-   Accuracy
-   Precision
-   Recall
-   F1-score

A comparison table is generated to summarize performance across models.

------------------------------------------------------------------------

## Results Summary

Among the three models tested, Support Vector Machine achieved the
highest overall accuracy, followed closely by Logistic Regression. Naive
Bayes also performed well but showed slightly lower recall for the SPORT
category.

------------------------------------------------------------------------

## How to Run

1.  Install required libraries: pip install scikit-learn pandas
    matplotlib seaborn

2.  Run the script: python sport_politics_classifier.py

------------------------------------------------------------------------

## Limitations

-   The dataset contains only English text.
-   The classification task is binary (SPORT vs POLITICS).
-   Real-world text may contain mixed topics.
-   TF-IDF does not capture deeper semantic meaning beyond word
    frequency patterns.

------------------------------------------------------------------------

## Conclusion

This project demonstrates how traditional machine learning algorithms
can effectively classify high-dimensional text data. The comparison
highlights that linear classifiers such as SVM and Logistic Regression
perform strongly for text categorization tasks.
