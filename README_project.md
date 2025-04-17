# Movie Recommendation System
# 🎬 Movie Recommendation System

This project is a simple yet effective *movie recommendation system* built using Python. It explores *content-based filtering* and *collaborative filtering* to recommend movies to users based on movie metadata and simulated user preferences.

## 📌 Problem Statement

With thousands of movies available, users often struggle to find what to watch next. This project solves that by recommending similar movies based on either the content of a selected movie or user preferences.

## 📊 Dataset

The dataset used is from *The Movie Database (TMDb)* and contains:

- id: Movie ID
- title: Movie title
- overview: Short movie description
- genres: Genre tags
- vote_average: Average rating
- vote_count: Number of votes
- popularity: Popularity score
- adult: Whether it's an adult film

## Data Cleaning & Feature Engineering

- Removed irrelevant columns
- Filtered movies based on vote count
- Created new features like description, vote_ratio
- Encoded categorical data
- Built user-item matrix for collaborative filtering

## Recommendation Techniques

### 1. Content-Based Filtering
- Uses *TF-IDF vectorization* on the movie overview text.
- Computes cosine similarity between movie plots.
- Recommends movies that are textually similar to a selected one.

### 2. 👥 Collaborative Filtering (Item-Based)
- Simulates *user-movie ratings* for 1000 users.
- Builds a *user-item matrix* using synthetic ratings.
- Recommends movies that are similar based on user preferences using *cosine similarity*.

## ⚙ Tools and Libraries

- Python (Jupyter Notebook)
- pandas, numpy
- sklearn (for vectorization, model training)
- matplotlib, seaborn (for visualization)

## Model Evaluation

### Classification Model (if used)
If a classifier (like logistic regression) was trained:

- *Accuracy*: 0.XX
- *Precision*: 0.XX
- *Recall*: 0.XX
- *F1 Score*: 0.XX

### Content-Based Results (Sample)
For the movie *Inception*, similar recommendations:

- Shutter Island  
- Interstellar  
- The Matrix  
- Source Code  

### Collaborative Filtering Results (Sample)
For a movie in the user-item matrix:

- Recommended: Movie A, Movie B, Movie C, ...

## 🗂 Project Structure
 
