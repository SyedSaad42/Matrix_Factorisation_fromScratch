Movie Recommendation System using Matrix Factorization (SVD)


**Overview**

This project implements a Movie Recommendation System from scratch using Matrix Factorization (MF) with Singular Value Decomposition (SVD).
The system predicts user preferences for movies by decomposing the user-item interaction matrix into latent factors that capture hidden patterns in the data.

The project was built without using high-level recommendation libraries, to strengthen the understanding of the mathematical foundations behind recommendation systems.

**Features**

Implemented Matrix Factorization with SVD from scratch.

Learns latent features for both users and items.

Predicts user ratings for unseen movies.

Handles sparse user-item rating matrices.

Provides movie recommendations based on predicted ratings.

**Tech Stack**

Language: Python

**Libraries:**

numpy for linear algebra and matrix operations

pandas for dataset handling

**Dataset**

The system was trained and tested using the MovieLens dataset, which contains user ratings for movies.

Each row contains: userId, movieId, rating, and timestamp.

Movie metadata (title, genres) was used for mapping recommendations to actual movie names.

Methodology

Data Preprocessing

Constructed a user-item rating matrix from the dataset.

Handled missing values by representing them as 0.

Matrix Factorization using SVD

Decomposed the user-item rating matrix into three matrices:

U (user feature matrix)

Σ (singular values)

V^T (item feature matrix)

Reduced dimensions to capture latent factors while avoiding noise.

Prediction

Reconstructed the approximated rating matrix.

Predicted missing ratings based on latent features.

Evaluation

Used Root Mean Squared Error (RMSE) to evaluate prediction accuracy.

Results

Achieved good reconstruction accuracy on the MovieLens dataset.

The system successfully recommends movies to users based on latent features, even if they have not rated those movies before.
