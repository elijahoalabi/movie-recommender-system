# Movie Recommender System

This project implements two recommender system approaches for movies:
1. **Content-Based Filtering** – recommends movies similar to ones the user already enjoyed, based on rating patterns.
2. **Collaborative Filtering** – recommends movies by analyzing similarities between users’ preferences.

The project uses the [MovieLens dataset](https://www.kaggle.com/datasets/grouplens/movielens-20m-dataset) and demonstrates how recommender systems can enhance personalization in digital platforms.

---


- **Content-Based Filtering**
  - Builds a user-item rating matrix.
  - Computes cosine similarity between movies.
  - Provides top-N movie recommendations based on similarity scores.
  - Uses fuzzy string matching to handle variations in input movie names.

- **Collaborative Filtering**
  - Implements user-user similarity using KNN from the `surprise` library.
  - Predicts ratings for unseen movies and recommends the top-N items.
  - Evaluated using:
    - RMSE
    - MAE
    - Precision@5
    - Recall@5



Content-Based: Effective at finding movies with similar characteristics but may lack diversity (recommends too many similar films).

Collaborative: Captures shared preferences among users, offering more diverse recommendations, but can struggle with data sparsity or cold start users.
