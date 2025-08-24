**Correlation-Based Movie Recommendation System
Overview**

This project implements a user-item collaborative filtering recommendation system using the MovieLens dataset.
The system recommends movies based on correlation of user ratings, identifying relationships between movies by analyzing rating patterns.

**Features**

Uses MovieLens dataset for user and movie rating data.

Computes average ratings and number of ratings per movie.

Generates movie-to-movie similarity using Pearson correlation.

Provides recommendations for a target movie based on highest correlated movies.

**Technologies Used**

Python

Pandas

NumPy

Matplotlib / Seaborn (for visualization)

Jupyter Notebook (development and testing)
**
How It Works**

Load the MovieLens dataset into a Pandas DataFrame.

Group data by movie titles to calculate mean ratings and number of ratings.

Build a user-item matrix of ratings.

Compute correlation between movies based on user ratings.

Return a ranked list of similar movies for a given title.

**Example**

If the target movie is Star Wars (1977), the system finds other movies that users who liked Star Wars also rated highly, and recommends them in descending order of correlation.

**Usage
**
Run the Jupyter Notebook or Python script to:

Explore data analysis and visualizations.

Generate recommendations by providing a target movie name.

**Future Improvements**


Implement matrix factorization methods (SVD, ALS) for deeper recommendation.

Incorporate additional metadata (genres, tags) for content-based filtering.

Build a web-based interface for interactive recommendations.
