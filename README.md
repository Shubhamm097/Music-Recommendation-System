# Music Recommendation System

## Table of Contents
  * [Overview](#overview)
  * [Motivation](#motivation)
  * [Approach](#approach)
  * [Run](#run)
  * [Bug / Feature Request](#bug---feature-request)
  * [Technology Stack](#technology-stack)
  * [Credits](#credits)


## Overview
This project is a step to deep dive in the recommendation systems that big tech giants like Netflix, Spotify, Reddit etc uses. I have built my own music recommendation system using [Kaggle Spotify Dataset]. The dataset consists of features that are extracted from the .wav files of the song. The system suggests top 10 recommendations after giving a song as input.

## Motivation
It is good to know what's going under the hood behind the famous apps that you are using. Apps like Spotify, Netfilx, Reddit has an elegant recommendation system that provides us with pretty good results and help us in exploring new songs/podcast in case of Spotify by manipulating our data. Thus, I have also built a basic recommendation system using cosine similarity.

## Approach
Recommendation System can be built in a couple of ways. A buncf of ways are listed below.
1. Reddit uses an algorithm to rank the news instead of using complex models using neural networks. Algorithm in recommendation could prove out to be effective than deep learning models as they can introduce the biasness for user, not recommending him the news of genre that the user has not seen yet but could be interested in.

2. The other way is using matrix and dividing the movies for example in different genres like comedy, thriller etc. Now, this matrix is initialised with random movies but as the time passes the matrix reflect the user's choice.

3. One another way is to not only just take the user's input to recommend him the movies but also other user's that has somewhat similar matrix to suggest movies to one another.

In my case, I do not have user base pre-built, so, I have to come up with either some sort of algorithm to recommend the music to user. I have used cosine similarity for this project. Cosine similarity is basically a dot product between two vectors. Thus, here, the vector is the features and in order to recommend I have taken dot product of the input song with all the songs in the dataset and return the top 10 similar songs.

## Run
After downloading the dataset from [here](https://www.kaggle.com/yamaerenay/spotify-dataset-19212020-160k-tracks), open a google colab/jupyter notebook and run the cells.


## Bug / Feature Request
If you'd like to request a new feature/approach, feel free to do so by opening an issue [here](https://github.com/Shubhamm097/Music-Recommendation-System/issues/new). Please include the relevant reasons for the feature or approach.

## Technology Stack
1. Python
2. Cosine Similarity
3. Sklearn


## Credits
- [Understand Recommendation Systems](https://towardsdatascience.com/introduction-to-recommender-systems-6c66cf15ada)

- [Kaggle Dataset for Spotify consisting 160k+ tracks](https://www.kaggle.com/yamaerenay/spotify-dataset-19212020-160k-tracks)

- [Reddit's Recommendation System](https://www.reddit.com/r/learnprogramming/comments/3a5oz8/recommendation_system_how_do_they_work/)

- [Spotify's Recommendation System](https://towardsdatascience.com/how-spotify-recommends-your-new-favorite-artist-8c1850512af0#:~:text=Well%2C%20Spotify's%20recommender%20system%20provides,it%20deems%20%E2%80%9Csimilar%E2%80%9D%20users.)
