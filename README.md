# Book-Recommendation-system-
A machine Learning model to recommends books using K-Means clustering and Cosine similarities 

# 📚 Hybrid Book Recommendation System

## 📝 Project Overview

This project presents a **hybrid book recommendation system** that aims to provide personalized book suggestions to users by combining clustering techniques and collaborative filtering. The system is built using a cleaned and filtered dataset containing user ratings and metadata about books such as titles, authors, and genres.

The primary objective is to segment users based on their reading preferences using **K-Means clustering**, and within these segments, identify books that are most relevant through **similarity-based recommendation techniques**.

---

## 🎯 Objectives

- To analyze user-book interaction data and derive meaningful patterns.
- To build a recommendation system that combines clustering with similarity-based techniques.
- To improve personalization by narrowing recommendations within user clusters.

---

## 📌 Methodology

1. **Data Preprocessing**  
   The dataset is cleaned to remove noise and inconsistencies. Unnecessary columns are dropped, and missing values are handled. Duplicate entries are removed to ensure the integrity of the recommendation process.

2. **User-Item Matrix Construction**  
   A matrix is created where rows represent users and columns represent books, with the values indicating user ratings. This matrix is further refined to retain only active users and frequently rated books.

3. **K-Means Clustering**  
   Users are clustered based on their rating patterns. The Elbow Method is used to determine the optimal number of clusters. This allows segmentation of users into groups with similar interests.

4. **Recommendation Engine**  
   For a given user, the system identifies the cluster they belong to and recommends books that are highly rated within that cluster. Cosine similarity is used to find books that are similar in terms of user engagement.

---

## 📁 Dataset Description

- **Name:** `filtered_books_dataset.csv`
- **Attributes:** Book Title, Author, Genre, Rating, User ID, etc.
- **Source:** Preprocessed version of a publicly available books dataset (e.g., Goodreads)

---

## 📚 Libraries & Tools Used

- **Programming Language:** Python
- **Libraries:**  
  - `pandas`, `numpy` – Data manipulation  
  - `scikit-learn` – Clustering and similarity computation  
  - `matplotlib`, `seaborn` – Data visualization  
  - `scipy` – Cosine similarity

---

## ✅ Outcomes

- The system successfully segments users and generates personalized book suggestions.
- It enhances user experience by filtering recommendations to a narrower and more relevant cluster.
- The hybrid approach improves recommendation accuracy compared to purely collaborative methods.

---

## 🧠 Future Scope

- Integration of Natural Language Processing (NLP) for content-based filtering using book descriptions or reviews.
- Deployment of the recommendation engine using a web interface (e.g., Streamlit).
- Incorporation of real-time user feedback to adapt recommendations dynamically.


