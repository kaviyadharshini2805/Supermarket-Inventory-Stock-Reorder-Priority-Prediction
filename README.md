# 🛒 Supermarket Inventory Clustering App

This Streamlit application predicts which cluster/category an inventory item belongs to using a pre-trained K-Means clustering model. It helps supermarket managers identify items with high, medium, or low stock priority.

## 🚀 Features

Simple and interactive Streamlit UI

Predicts item cluster using K-Means

Uses scaler and encodings consistent with training

Supports category & supplier dropdowns

Provides cluster interpretation:

🟢 High Stock – Low Reorder Risk

🟡 Moderate Stock – Medium Reorder Risk

🔴 Low Stock – High Reorder Priority

## 📂 Project Structure

  ├── kmeans_inventory_model.joblib
  
  ├── inventory_scaler.joblib

  ├── train.py
  
  ├── supermarket_inventory.xlsx  
  
  └── app.py

## 🧠 How It Works

User enters item details (Stock, Reorder Level, Unit Price, Category, Supplier).

Categorical values are encoded to match training.

Input is scaled using the saved scaler.

K-Means predicts the cluster.

The app displays the cluster and a readable interpretation.

## 🛠️ Installation
pip install streamlit pandas joblib

## ▶️ Running the App
streamlit run app.py

## 📌 Requirements

Python 3.8+

Streamlit

Pandas

Joblib

Pre-trained model + scaler
