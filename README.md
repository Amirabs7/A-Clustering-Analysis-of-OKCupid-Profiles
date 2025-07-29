# A-Clustering-Analysis-of-OKCupid-Profiles
🧠 Project Overview
This project explores a real-world dataset from OKCupid, a dating app that stands out for its user-matching algorithm based on optional personality and lifestyle questions. Using a combination of exploratory data analysis (EDA), dimensionality reduction (UMAP), and clustering (KMeans), we uncover insights about user profiles and behavioral patterns.

Dataset Source:
 https://www.kaggle.com/datasets/andrewmvd/okcupid-profiles/data
 
🧼 Data Cleaning & Preparation
Dropped columns with excessive missing values (e.g., religion, pets, essay answers).

Handled missing values in key lifestyle/demographic columns with "unknown" fillers.

Encoded categorical variables for modeling (e.g., sex, orientation, education).

Filtered income and height for reasonable ranges.



📊 Exploratory Data Analysis (EDA)
Distributions: Age, income, education, and body type distributions reveal majority trends.

Cross-Analysis: Showed relationships between drinking habits and income or orientation.

Encoding Example: Translated qualitative drink frequency to numerical scale for better analysis.

📉 Dimensionality Reduction with UMAP
UMAP projected multi-dimensional user data (age, income, height, encoded sex) into 2D for visualization:


📦 Clustering with KMeans
Clustered profiles into 5 user groups

Evaluated clustering with Silhouette Score

Cluster 1 emerged as dominant: Younger (avg. age ~32) , Highly educated , Very low income


📌 Ideas to Extend
Add NLP sentiment analysis on essays if re-included

Predict matching compatibility using classification

Use UMAP+HDBSCAN for more organic clusters

Expand clustering with more psychological/lifestyle variables (e.g. sign, drugs, speaks)

Refine clustering with DBSCAN or HDBSCAN for non-spherical clusters


