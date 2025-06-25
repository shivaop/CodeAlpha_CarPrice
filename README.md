# 🚗 Car Price Prediction using Machine Learning

![banner](https://img.freepik.com/free-vector/automobile-sales-abstract-concept-illustration_335657-4132.jpg?w=1060&t=st=1719311114~exp=1719311714~hmac=cfca92a183ee4d58fbd74ea66a95c5e0ec8be6480b00c3d3e03ec7f88b1f1874)

## 📌 Project Overview

This project aims to predict the selling price of used cars using Machine Learning. We explore and preprocess the data, reduce dimensions using PCA, and build the foundation for a predictive model.  

> **Goal:** Help users estimate a fair selling price for second-hand cars based on features like age, brand, fuel type, and more.

---

## 📂 Dataset

- **File:** `car data.csv`
- **Source:** Provided by CodeAlpha Internship
- **Features:**
  - `Present_Price`, `Kms_Driven`, `Fuel_Type`, `Seller_Type`, `Transmission`, `Owner`, etc.

---

## 🔍 Exploratory Data Analysis

- Checked for nulls and duplicates
- Visualized correlations using heatmaps
- Encoded categorical variables
- Used PCA to reduce dimensionality for better efficiency

---

## 📉 Dimensionality Reduction

We applied **PCA (Principal Component Analysis)** to compress the dataset while preserving maximum variance.

```python
from sklearn.decomposition import PCA
pca = PCA(n_components=5)
X_pca = pca.fit_transform(X_scaled)
