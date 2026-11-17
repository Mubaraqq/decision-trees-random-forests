# Decision Trees & Random Forests: Rain Prediction

## Overview
This notebook explores tree-based machine learning models (Decision Trees and Random Forests) to predict if it will rain tomorrow in Australia. It covers the complete ML pipeline, including hyperparameter tuning and handling overfitting.

## Dataset
- **Source:** Kaggle (Rain in Australia)
- **Goal:** Binary Classification (Predict "Yes" or "No" for RainTomorrow)
- **Size:** ~145,000 rows, 23 columns

## What's Covered:
- **Data Preprocessing:** Time-based splitting, imputation, scaling, and one-hot encoding.
- **Decision Trees:** Training a single tree, visualizing it, and understanding the Gini index.
- **Overfitting:** Demonstrating how a single tree memorizes data (99.9% train accuracy, 79% val accuracy).
- **Hyperparameter Tuning:** Using `max_depth`, `max_leaf_nodes`, `max_features`, and `min_samples_split` to find the sweet spot.
- **Random Forests:** Combining 100+ trees to cancel out errors and improve validation accuracy.
- **Feature Importance:** Comparing how a single tree relies heavily on one feature vs. a forest relying on a team effort.

## Key Learnings
- **Overfitting is the enemy:** A single tree will memorize the data. We must limit its depth or use a forest.
- **The U-shaped curve:** Tuning hyperparameters is a trade-off between underfitting (too simple) and overfitting (too complex).
- **Wisdom of the Crowd:** Random Forests work by averaging the predictions of many diverse trees. 
- **The Noise Ceiling:** Weather prediction is inherently chaotic. Hyperparameter tuning has diminishing returns once the model hits the data's natural accuracy limit (~85.6%).

## Technologies Used
- Python
- Pandas & NumPy
- Scikit-learn
- Matplotlib & Seaborn
