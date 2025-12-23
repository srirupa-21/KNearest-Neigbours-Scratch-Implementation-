# KNearest-Neigbours-Scratch-Implementation

## 💎 Diamond Price Prediction using KNN (From Scratch)

This project demonstrates how to **predict diamond prices** using the **K-Nearest Neighbors (KNN)** algorithm implemented **from scratch**, and compares its performance with **scikit-learn’s KNN implementation**.

The goal of this project is to deeply understand how KNN works internally, especially for **regression problems**, while following a proper **machine learning pipeline**.

---

## 📌 Project Overview

- **Problem Type:** Regression
- **Algorithm Used:** K-Nearest Neighbors (KNN)
- **Dataset:** Diamonds dataset
- **Target Variable:** `price`
- **Evaluation Metrics:** MAE, RMSE, R² Score

---

## 🧠 Key Learning Objectives

- Understand distance-based learning
- Implement KNN algorithm **from scratch**
- Handle categorical and numerical data correctly
- Prevent data leakage during preprocessing
- Compare scratch implementation with sklearn’s optimized model

---


## ⚙️ Step-by-Step Implementation

### Step 1: Load the Dataset
- Load the diamonds dataset using pandas

### Step 2: Identify Features and Target
- **Features (X):** carat, cut, color, clarity, depth, table, x, y, z
- **Target (y):** price

### Step 3: Train-Test Split
- Split data into **75% training** and **25% testing**

### Step 4: Data Preprocessing (Training Data)
- **Categorical Encoding:** One-Hot Encoding (`cut`, `color`, `clarity`)
- **Numerical Scaling:** StandardScaler
- Implemented using `ColumnTransformer`

### Step 5: Data Preprocessing (Test Data)
- Apply the same transformations using `transform()` only

### Step 6: KNN from Scratch
- Implemented Euclidean distance manually
- Predicted prices using mean of nearest neighbors
- No use of sklearn’s KNN in this step

### Step 7: Model Evaluation
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

### Step 8: Sklearn KNN Comparison
- Train `KNeighborsRegressor`
- Compare results with scratch implementation

---

## 🧮 Why Scaling & Encoding Are Important

- KNN is a **distance-based algorithm**
- Feature scaling ensures no feature dominates distance
- One-hot encoding avoids introducing artificial ordering in categorical data

---

## 🛠️ Libraries Used

- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib (optional for visualization)

---
