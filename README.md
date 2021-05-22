## Movie Recommender Systems

GroupLens Research has collected and made available rating data sets from the MovieLens web site (http://movielens.org). 
The data sets were collected over various periods of time, depending on the size of the set.

Recommendation Engines try to make a product or service recommendation to people. In a way, Recommenders try to narrow down choices for people by presenting them with suggestions that they are most likely to buy or use.
These datasets can be used to model and recommend users with the movie choices based on their interest. we have used Content based, Collaborative based and Hybrid models to implement the recommendation system.
We have used surprise API to measure the RMSE and the acuracy of the model. 

## Details about Dataset

#### Datasets:

1) we have used Movie lens dataset for the building recommender systems 
2) Dataset can be downloaded from link: https://www.kaggle.com/rounakbanik/the-movies-dataset

## Types of data:

Full dataset: This dataset consists of 26,000,000 ratings by 270,000 users for 45,000 movies.

Sample dataset: we have taken The subset of 100,000 ratings from 700 users on 9,000 movies for building recommender system.

## Data description:

The data are contained in the following files:

1) credits.csv             --> This dataset contains columns - cast, crew, ID
2) keywords.csv            --> This dataset contains columns - id, keywords
3) links_small.csv         --> This dataset contains columns - movieId, imdbId, tmdbId
4) movies_metadata.csv     --> This dataset contains columns - adult, belongs_to_collection, budget, genres, homepage, id, imdb_id, original_language, original_title, overview, release_date, revenue, runtime, spoken_languages, status, tagline, title, video, vote_average, vote_count
5) ratings_small.csv       --> This dataset contains columns - userId, movieId, rating, timestamp
6) ratings.csv             --> This dataset contains columns - adult, belongs_to_collection, budget, genres, homepage, id, imdb_id, original_language, original_title, overview, release_date, revenue, runtime, spoken_languages, status, tagline, title, video, vote_average, vote_count

## Code

Jupiter notebooks and script have been developed for this project.
After pre-processing the dataset we have done the following analysis with the proposed models:

Content Based Model: Content based recommendation model by Using movie description & taglines. We have used TF-IDF to implemt this model. 

Colloborative Model: Colloborative based by Using movie description,taglines,keywords, cast, director and genres. By using all these variables We have implemented the 
Item-Based Collaborate filtering. 

Suprise Library: we have used Collaborate filtering using Suprise Library API to measure the RMSE and Acuuracy.

Hybrid Model: By using the features from content based and Colloborative models we have implemented Hybrid Recommendation System.


## Dependencies:

Jupyter Notebook
Python >=3.5
pandas
numpy
scipy
ast module
nltk
scikit-learn
scikit-surprise
