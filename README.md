# 💘 A Clustering Analysis of OKCupid Profiles

This project explores a rich dataset from **OKCupid**, a dating app known for its compatibility matching system based on optional personality and lifestyle questions. The data contains over **60,000 user profiles**, including demographics, lifestyle preferences, and free-text essays.

We use **exploratory data analysis (EDA)**, **dimensionality reduction (UMAP)**, and **KMeans clustering** to identify distinct dating archetypes. The goal: uncover how people present themselves—and how they cluster—on a major online dating platform.

📅 **Dataset Source**:  
Kaggle – [`OKCupid Profiles`](https://www.kaggle.com/datasets/andrewmvd/okcupid-profiles/data)  
🗓️ Year Collected: 2018  
📦 Records: ~60,000 user profiles (structured + text data)

---

## What this project shows
- Text and clustering analysis using Python (pandas, scikit-learn, UMAP, KMeans).
- Patterns in dating profiles and traits across demographics.
- Reproducible project with clear visualizations and interactive insights

---

## 📁 Repository Structure

   ├── Age distribution.png 
   ├── Age distribution per gender.png 
   ├── Body type distribution.png 
   ├── Drinking frequency by sexual orientation.png 
   ├── Education level distribution.png 
   ├── Income distribution.png 
   ├── Median income by education levels.png 
   ├── uncovering_dating_archetypes_clustering_okcupid_profiles_using_umap_and_kmeans.py 
   └── README.md ``` </pre>

---

## 🧼 Data Cleaning & Preparation

- ❌ **Dropped** columns with excessive missing values: `religion`, `pets`, `essay*`
- 🕳️ **Filled missing** lifestyle values with `"unknown"`
- 🔤 **Encoded** categorical data: `sex`, `orientation`, `education`
- 🧹 **Filtered** height and income values to remove unrealistic entries

---

## 📊 Exploratory Data Analysis (EDA)

We explored user traits and behavioral patterns across multiple axes:

### ✅ **Key Observations**:

- **Most users are in their 20s and early 30s**
- **Women report lower income than men on average**
- **Higher education levels are associated with slightly higher income**, but many users with Master's degrees still report low income
- **People who drink frequently are more likely to be straight and higher earners**

### 📁 Visual Highlights:

- `Drinking frequency by sexual orientation`
- `Median income by education levels`
- `Age distribution per gender`

---

## 📉 Dimensionality Reduction with UMAP

We applied **UMAP** to reduce high-dimensional data (age, income, sex, height) into **2D space** for cluster visualization.

- 🔍 Maintains local structure
- 📊 Makes clusters visually interpretable
- 🧩 Prepares data for clustering

---

## 📊 Key Visualizations

### Body Type Distribution
![Body Type Distribution](https://raw.githubusercontent.com/Amirabs7/A-Clustering-Analysis-of-OKCupid-Profiles/main/Body%20type%20distribution.png)

### Drinking Frequency by Sexual Orientation
![Drinking Frequency](https://raw.githubusercontent.com/Amirabs7/A-Clustering-Analysis-of-OKCupid-Profiles/main/Drinking%20frequency%20by%20sexual%20orientation.png)

### Income Distribution
![Income Distribution](https://raw.githubusercontent.com/Amirabs7/A-Clustering-Analysis-of-OKCupid-Profiles/main/Income%20distribution.png)

---



## 📦 Clustering with KMeans

We used **KMeans clustering** (k=5) on the UMAP-reduced data.

### ⭐ **Key Findings from Clustering**:

1. **Cluster 1**:  
   - 🎓 **Highly educated**  
   - 🧑‍🎓 **Young (avg. age ~32)**  
   - 💸 **Very low income** → *Educated but under-earning*
  
2. **Cluster 2**:  
   - 🧔‍♂️ **Older males**  
   - 🥂 **Frequent drinkers**  
   - 💵 **Mid to high income**

3. **Cluster 3**:  
   - 🚭 **Non-drinkers**  
   - ✝️ **Often religious or conservative lifestyle markers**  
   - 👥 **More gender balance**

> Clusters capture **real behavioral archetypes** in the dating world—not just random groupings.

---

## 🔮 Future Extensions

- 📝 **Add NLP**: Analyze user essays (sentiment, topic modeling)
- ❤️ **Matching prediction**: Train model to predict compatibility
- 🧠 **Better clustering**:
  - Try **HDBSCAN** for organic shapes  
  - Include more lifestyle traits (e.g., `drugs`, `sign`, `speaks`)
- 🧪 Refine feature scaling + distance metrics

---

## 🛠️ How to Reproduce
1. Clone this repository:
git clone https://github.com/Amirabs7/OKCupid-Analysis.git

---



## 👩‍💻 Author
**Amira Ben Salem**  
📫 Email: besamira77@gmail.com  
📍 Berlin, Germany  

---
