**Sentiment Analysis Project**

**Project Overview**
This project focuses on building a text classification system to analyze sentiment from movie reviews using the IMDb dataset. 
The goal is to work with data, train the model ,to compare different machine learning models and determine which performs best for sentiment classification.

**Dataset**

We used the IMDb dataset from https://www.kaggle.com/datasets/pawankumargunjan/imdb-review, which contains movie reviews labeled as positive or negative.
To enhance the analysis, we also added a neutral category by sampling additional data.

Dataset splits:

Training set: used to train the models

Test set: used to evaluate the models

Unsupervised data: used to generate neutral samples

**Data Preprocessing**

Before training, text data underwent cleaning and normalization:

Converted text to lowercase

Removed stopwords (common words that do not add meaning, e.g., “the”, “and”)

Lemmatization: reduced words to their base form (e.g., “running” → “run”)

Removed non-alphabetic characters

This ensures the model learns from meaningful words and not noise.

**Categories**

We defined three sentiment categories:

Negative (0)

Positive (1)

Neutral (2)

The data was balanced with equal samples from each category.

**Train/Test Split**

The dataset was split into training and testing sets:

Training set: used to train models

Test set: used to evaluate model performance

**Models Used**

We implemented and compared two classification approaches:

TF-IDF + Logistic Regression

TF-IDF vectorization transforms text into numerical feature vectors

Logistic Regression is used to classify these vectors into sentiment categories

TF-IDF + Support Vector Machine (SVM)

Same TF-IDF features

SVM classifier with a linear kernel

**Model Comparison**

We evaluated models using metrics:

Precision

Recall

F1-score

Accuracy
We also visualized results with confusion matrices.

**Summary of results:**

TF-IDF + Logistic Regression: fast, interpretable, achieved higher recall and accuracy overall

TF-IDF + SVM: slightly slower, performed similarly in accuracy but required more computation

Conclusion: Logistic Regression performed slightly better in terms of speed and accuracy for this dataset.
