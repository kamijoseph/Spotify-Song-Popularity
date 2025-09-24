# Spotify Song Popularity

This project explores predicting the popularity of songs on Spotify using machine learning models. It combines audio features and metadata with various ML techniques to evaluate which models perform best for regression tasks.

## Overview

Dataset sourced via Spotify API (≈ 81k tracks after cleaning).

### Target:
popularity score (0–100).

### Features:
song metadata (artists, track names), audio features (danceability, energy, tempo, etc.).

### Models explored:

Linear Regression

Random Forest Regressor

XGBoost, LightGBM, CatBoost (tree-based boosting models)

## Data Preparation

Removed duplicate tracks and invalid entries.

Final dataset size: ~81,344 songs.

Features preprocessed: one-hot encoding for categorical variables, scaling for neural networks.

Tree-based models trained on raw features (no scaling required).


## Tools & Libraries

Explore the *requirements.txt* file

## Challenges & Solutions

### Large dataset handling:
optimized with efficient pandas operations.

### Duplicate removal:
used drop_duplicates() on track/artist features.

### model Exploration
explored different models and their tuning to increase perfomancr

## Future Work

Hyperparameter tuning with GridSearch/Optuna.

Deploy model as a Flask/FastAPI web app for song popularity prediction.

Explore recommendation-based tasks (playlist or artist-level).

## License

This project is licensed under the MIT License.