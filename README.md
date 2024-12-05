# CineRec

CineRec is a movie recommendation application that provides detailed information about requested movies, including their synopsis, genres, release date, ratings, runtime, top cast, user reviews, recommended movies, and more.

The application fetches movie-related data (such as title, genre, runtime, ratings, posters, etc.) using the TMDB, https://www.themoviedb.org and performed sentiment analysis on those reviews.

## Finding similar movies
### Without Content-Based Analysis (Ratings-Based)

In this method, movies with similar ratings are identified using the K-Nearest Neighbors (KNN) algorithm.
### Content-Based Analysis

This approach leverages movie information, such as genres, to determine the most similar movies.

## Matrix Factorisation(Collabarative Filtering) 

Two approaches were tried to do matrix factorisation

### Low-Rank Approximation: Although effective, this method was slower in execution.
### Sparse Matrix Factorization using Scipy’s SVD: A more efficient solution that handles sparse matrices effectively.


## Deep Learning Methods

Matrix factorization is a widely used method in recommendation systems. It is based on learning low-dimensional embeddings for both users and movies.
For instance, embeddings for movies might encode features like the amount of action or runtime, while embeddings for users might capture preferences for action or long movies. Combining these embeddings enables predictions of ratings for unseen movies.

### 1.Matrix Factorization with Deep Learning
### 2. Matrix Factorization with Non-Negative Embeddings
### 3. Advanced Neural Networks featuring different embedding configurations for users and movies.

## Required Tools

1. Python 3
2. Keras
3. Scipy
4. Numpy
5. Pandas

### Sources of the datasets 

1. [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset)
2. [List of movies in 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
3. [List of movies in 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
4. [List of movies in 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)


