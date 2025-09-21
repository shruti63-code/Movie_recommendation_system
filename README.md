# Movie_recommendation_system
🎬 Movie Recommendation System

This project implements a Movie Recommendation System using Collaborative Filtering in Python. It uses the MovieLens-style dataset (movies.csv and ratings.csv) to recommend movies to users based on similar users' preferences.

📌 Features

Collaborative Filtering (User-User Similarity using cosine similarity).

Recommends movies to a user based on ratings from similar users.

Works with movies.csv and ratings.csv datasets.

Simple, lightweight, and runs in Google Colab (Python 3 runtime).

📂 Dataset

movies.csv → Contains movieId, title, and genres.

ratings.csv → Contains userId, movieId, rating.

Example:

movies.csv

movieId,title,genres
1,Toy Story (1995),Adventure|Animation|Children|Comedy|Fantasy
2,Jumanji (1995),Adventure|Children|Fantasy
3,Grumpier Old Men (1995),Comedy|Romance


ratings.csv

userId,movieId,rating
1,1,4.0
1,3,3.5
2,1,5.0
2,2,4.5
3,2,4.0

🚀 Installation & Setup

Open Google Colab and create a new Python 3 notebook.

Upload the dataset files (movies.csv and ratings.csv).

Copy and paste the code from this repo into your notebook.

Run the notebook to generate recommendations.

🧠 How It Works

Load and merge movies and ratings datasets.

Create a User-Movie Rating Matrix.

Compute Cosine Similarity between users.

For a target user:

Find similar users.

Aggregate ratings from similar users (weighted by similarity).

Recommend top movies the target user hasn’t rated yet.

📊 Example Output
Top movie recommendations for User 1:
Jumanji (1995)                 8.75
Grumpier Old Men (1995)        6.30
Toy Story (1995)               5.90
📦 Requirements
Python 3.x

pandas

numpy

scikit-learn

Install dependencies (if running locally):

