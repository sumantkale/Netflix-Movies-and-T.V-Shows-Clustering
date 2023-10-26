# Netflix Movies and TV Shows Clustering

This repository contains the code and resources for a project focused on clustering Netflix movies and TV shows. The primary objective of this project is to classify and group Netflix content into clusters based on their attributes, with the aim of providing valuable insights and recommendations to users.

## Project Overview

- **Problem Statement**: In this project, we aim to categorize Netflix shows into clusters, ensuring that shows within the same cluster are similar to each other while being dissimilar to those in other clusters.

- **Dataset**: The dataset used contains approximately 7,787 records and 12 attributes. Our initial steps involve data preprocessing and exploratory data analysis (EDA).

- **Key Insights**:
  - Netflix has a greater number of movies compared to TV shows.
  - The total number of shows added to Netflix is growing exponentially.
  - The majority of shows are produced in the United States.
  - Most Netflix shows are created for adults and young adults.

- **Data Preprocessing**: We preprocess the text data by removing punctuation and stop words. The processed data is then transformed into TF-IDF vectors to prepare for text-based clustering.

- **Clustering Attributes**: We cluster the data based on attributes such as director, cast, country, genre, and description. These attributes are tokenized, preprocessed, and vectorized using TF-IDF vectorization.

- **Dimensionality Reduction**: To address high dimensionality, we employ Principal Component Analysis (PCA) and reduce the number of components to 4,000, capturing over 80% of the variance.

- **Clustering Methods**: We implement two clustering algorithms:
  - K-means clustering with the optimal number of clusters determined using the elbow method and Silhouette score analysis (6 clusters).
  - Agglomerative clustering with the optimal number of clusters identified through dendrogram visualization (12 clusters).

- **Recommendation System**: A content-based recommender system is built using cosine similarity to provide users with 10 personalized show recommendations based on their viewing history.


