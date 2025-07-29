# A-Clustering-Analysis-of-OKCupid-Profiles
🧠 Project Overview
This project explores a real-world dataset from OKCupid, a dating app that stands out for its user-matching algorithm based on optional personality and lifestyle questions. Using a combination of exploratory data analysis (EDA), dimensionality reduction (UMAP), and clustering (KMeans), we uncover insights about user profiles and behavioral patterns.

Dataset Source:
Kaggle - OKCupid Profiles

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

Color-coded by sex

Clear visual separation among different clusters

Abstract space (X: -10 to 20, Y: -5 to 20) representing user similarity

📦 Clustering with KMeans
Clustered profiles into 5 user groups

Evaluated clustering with Silhouette Score

Cluster 1 emerged as dominant:

Younger (avg. age ~32)

Highly educated

Very low income

Balanced gender mix
🔍 Cluster Insights
Cluster	Avg Age	Income	Education	Smokes	Drinks	Sex Mix
1	32	$1,147	High	Moderate	Moderate	Mixed
2	29	$1M	High	High	Moderate	Slight Male Bias
0,3,4	33–36	$48K–$310K	Varied	Varied	Moderate	Mixed

Cluster 1 dominates the dataset — likely students, early-career professionals, or underpaid but educated individuals. Clusters 0,2,3,4 are more niche.

ools Used

Python (pandas, seaborn, matplotlib, scikit-learn, UMAP)

Jupyter Notebook / Google Colab

✅ Next Steps

Add interactivity with Streamlit (e.g. cluster explorer)

Expand clustering with more psychological/lifestyle variables (e.g. sign, drugs, speaks)

Refine clustering with DBSCAN or HDBSCAN for non-spherical clusters

Made by Amirabs7

