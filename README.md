# 🎮 Recommender System for Steam Games

## 📌 Overview

This project implements a **collaborative filtering recommender system** using the **ALS (Alternating Least Squares)** algorithm to suggest video games to users based on implicit behavior data from the Steam platform. It utilizes **PySpark** for scalable processing and **MLflow** for experiment tracking and model logging.

---

## 📊 Objective

- Explore the Steam gameplay dataset (`steam_200k.csv`)
- Preprocess and transform the data for collaborative filtering
- Train and tune an ALS-based recommendation model
- Evaluate model performance using cross-validation
- Generate game recommendations for users

---

## 🛠️ Technologies Used

- Python  
- PySpark (Spark MLlib)  
- MLflow (for experiment tracking)  
- Databricks Community Edition  

---

## 📁 Dataset

The dataset used (`steam_200k.csv`) includes:
- `user_id`: Unique identifier for each user
- `game_name`: Title of the game
- `behavior`: Type of interaction (e.g., play, purchase)
- `value`: Time played or purchase count

> Note: Only "play" behavior is used to model implicit user preferences.

---

## 🧪 Model & Evaluation

- **Algorithm**: ALS (from `pyspark.ml.recommendation`)
- **Tuning**: Grid Search with TrainValidationSplit and CrossValidator
- **Metrics**: RMSE (Root Mean Square Error)
- **Seed**: 42 for reproducibility

---

## 🚀 How to Run

1. Open the notebook in **Databricks Community Edition**
2. Upload the dataset (`steam_200k.csv`) to `/FileStore/tables/`
3. Run all cells sequentially
4. MLflow will track all runs and log model performance

---

## 📈 Results

- ALS model trained with optimized parameters via cross-validation
- Recommendations generated for sample users
- Experiment details and metrics logged to MLflow

---

## ✍️ Author

*Marvis Osazuwa*  
Course: Recommender Systems Assignment 

---

