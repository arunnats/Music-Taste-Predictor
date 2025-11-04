# 🎵 Music Taste Prediction using Regression on Spotify Dataset

## 📖 Problem Statement

In this project, we aim to build a **music taste prediction model** that can estimate how much a user might like a given song based on its audio features.  
Using the [Spotify Song Attributes Dataset](https://www.kaggle.com/datasets/geomack/spotifyclassification), we will train a **regression-based machine learning model** to predict a **"preference score"** (or likelihood of liking a song) based on numerical characteristics such as tempo, energy, danceability, loudness, and acousticness.

The goal is to model the relationship between a song’s measurable features and its perceived popularity or user preference, allowing us to **recommend songs aligned with a user’s taste** or **predict how appealing a new track might be**.

---

## 🎯 Objectives

- Explore and understand the Spotify dataset and its features.
- Clean and preprocess the data for regression modeling.
- Train and evaluate regression algorithms to predict song preference.
- Identify which audio features most strongly influence user taste.
- Demonstrate how such a model could be used to power a music recommender system.

---

## 🧠 Intent

This project focuses on **supervised machine learning**, specifically **regression modeling**, to understand and predict human preferences in music.  
Rather than relying on collaborative filtering or pre-trained neural networks, we directly train our model from scratch using numeric song attributes.

The intent is to:

- Apply core ML concepts (feature engineering, training/testing split, model evaluation).
- Use regression techniques to predict continuous outcomes (song likability or popularity score).
- Build an interpretable, data-driven system that can generalize to unseen songs.

---

## ⚙️ Methodology

1. **Data Collection & Loading**

   - Import the Spotify dataset from Kaggle.
   - Inspect the attributes such as `tempo`, `energy`, `loudness`, `acousticness`, `danceability`, `valence`, etc.

2. **Data Cleaning & Preprocessing**

   - Handle missing or inconsistent values.
   - Normalize or scale numerical features.
   - Encode categorical variables if any (e.g., genre).

3. **Feature Engineering**

   - Select relevant song-level attributes as predictors.
   - Optionally create derived features such as `tempo × energy` or `acousticness / loudness`.

4. **Model Training**

   - Split the dataset into training and testing sets (e.g., 80/20 split).
   - Train regression models such as:
     - **Linear Regression**
     - **Random Forest Regressor**
     - **XGBoost Regressor**
   - Tune hyperparameters and compare model performances.

5. **Evaluation**

   - Evaluate using metrics like **Mean Squared Error (MSE)** and **Root Mean Squared Error (RMSE)**.
   - Plot predicted vs. actual preference/popularity scores.
   - Analyze feature importances to understand what makes songs “likable.”

6. **Prediction & Recommendation**
   - Predict the likability score for unseen songs.
   - Recommend top songs based on predicted preference.

---

## 🧩 Expected Outcome

- A regression model capable of predicting how much a user (or general audience) might like a song based on its acoustic properties.
- Insights into which features (e.g., energy, tempo, danceability) most influence song appeal.
- A foundation for building personalized music recommendation systems.

---

## 🧰 Tools & Libraries

- **Python**
- **Pandas, NumPy** for data manipulation
- **Scikit-learn** for model training & evaluation
- **Matplotlib / Seaborn** for visualization
- **XGBoost / LightGBM** (optional) for advanced regression modeling

---
