## Exploratory Data Analysis and Modelling of Twitter Mental Health Disorders and Music Preferences for Machine Learning Applications


### Introduction

This project is done in scope of AIN423 - Data Intensive Applications Course at Hacettepe University. We aim to inspect the relationship between mental health disorders and music preferences by using Twitter data. We will use the data to create a machine learning model that can predict mental health disorders based on music preferences.

### Data

The data is open and accessible from the following link: https://www.kaggle.com/datasets/rrmartin/twitter-mental-disorder-tweets-and-musics .
We have used 2 csv files from the dataset which are anon_disorder_tweets.csv and anon_disorder_lyrics.csv . This data was scraped using TwitterAPI and GeniusAPI. The data contains tweets from users who have mental health disorders and their music preferences. The data is anonymized and contains null or recurring tweets.

### Methodology

We will use the following steps to create a machine learning model:

1. Exploratory Data Analysis
2. Feature Engineering
3. Modelling
4. Evaluation

### File Hierarchy

musics_eda.ipynb : Exploratory Data Analysis of the music data
tweets_eda.ipynb : Exploratory Data Analysis of the tweet data

text_processing.ipynb : Text processing of both tweet and music data

sampling/ : Contains the sampled data for the project
modelling/ : Contains the modelling code and results

modelling/lyrics_feature_extraction.ipynb : Feature extraction of the music data using the specified BERT model.
modelling/tweets_feature_extraction.ipynb : Feature extraction of the tweet data using the specified BERT model.

modelling/tweets_modelling_bert.ipynb : Modelling of the tweet data using features extracted from base BERT model.
modelling/tweets_modelling_mentalbert.ipynb : Modelling of the tweet data using features extracted from MentalBERT model.
modelling/tweets_modelling_multibert.ipynb : Modelling of the tweet data using features extracted from MultiBERT model.

modelling/musics_modelling.ipynb : Modelling of the music data using lyric-BERT model.

modelling/musics_feature_modelling.ipynb : Modelling of the music data using the **hand crafted features**.

### Results

We have achieved the following results:

- The best model for the tweet data is the MentalBERT model with an weighted f1-score as 0.20 .
- The best model for the music data is the lyric-BERT model with an weighted f1-score as 0.24 .

### Authors

- Alperen Demirci - 2220765010
- Bora Dere - 2220765021