

# Movie Recommender System

## Project Overview
This project implements a movie recommender system that suggests the 5 most similar movies based on the movie name entered. The system uses natural language processing (NLP) to analyze movie metadata and generate recommendations.

## Table of Contents
- Introduction
- Dataset
- Data Preprocessing
- Feature Engineering
- Recommendation System
- Conclusion

## Introduction
This project focuses on recommending movies by analyzing various attributes such as genres, keywords, cast, and crew. The goal is to enhance the user experience by providing personalized movie recommendations based on the similarity to a given movie.


## Datasets

Movies Data:
- budget
- genres
- homepage
- id
- keywords
- original_language
- original_title
- overview
- popularity
- production_companies
- production_countries
- release_date
- revenue
- runtime
- spoken_languages
- status
- tagline
- title
- vote_average
- vote_count
- Credits Data:

movie_id
- title
- cast
- crew

## Data Preprocessing
Steps involved in data preprocessing:

- Extract Relevant Information: Extracted names from genres, keywords, cast (top 3 actors), and crew (director).
- Text Processing: Converted strings to lists and removed extra spaces.
- Feature Combination: Created a new column tags by combining overview, genres, keywords, cast, and crew.
- Lowercasing and Lemmatization: Converted text to lowercase and applied stemming for uniformity.

## Feature Engineering
Feature engineering involved:

- Text Vectorization: Used CountVectorizer to convert text data into numerical vectors.
- Stemming: Applied Stemming to reduce words to their base form.

## Recommendation System
The recommendation system works as follows:

- Similarity Calculation: Uses cosine similarity to compute the similarity between movies based on the vectorized tags.
- Recommendation Function: recommend(movie) returns the 5 most similar movies to the entered movie name.

## Conclusion
The project successfully implements a movie recommender system that suggests the 5 most similar movies based on the entered movie name. This can enhance user experience by providing personalized recommendations.
