# 🎬 Movie Recommendation System

A content-based movie recommendation system built using Machine Learning that suggests movies similar to a selected movie based on story, genres, cast, keywords, and director. The project is also deployable as a Streamlit web application.

---

## 🚀 Project Overview

This system recommends movies by analyzing their content similarity rather than user ratings. It uses Natural Language Processing (NLP) and cosine similarity to find movies that are most similar to the one selected by the user.

Example:
If a user likes **Inception**, the system may recommend  
*Interstellar, The Prestige, Shutter Island*, etc.

---

## 🧠 Type of Recommendation System

**Content-Based Recommendation System**

- No user ratings required  
- Works well for new users (cold start problem)  
- Recommendations depend on movie metadata  

---

## 🛠️ Technologies Used

- Python  
- Pandas & NumPy  
- Scikit-learn  
- Streamlit  
- Pickle  

---

## 📂 Project Structure

movie-recommendation-system/
│
├── movie_recommender.ipynb
├── app.py
├── movies.pkl
├── requirements.txt
└── README.md

---

## ⚙️ How It Works

1. Movie metadata (overview, genres, keywords, cast, director) is combined into a single text field  
2. Text is converted into numerical vectors using **TF-IDF Vectorization**  
3. **Cosine Similarity** is used to measure similarity between movies  
4. The top 5 most similar movies are recommended  

---

## 🌐 Streamlit Web App

The Streamlit app allows users to:
- Select a movie from a dropdown  
- Click **Recommend**  
- Instantly view similar movie suggestions  

---

## ▶️ How to Run Locally

### Install dependencies
```bash
pip install -r requirements.txt
Run the Streamlit app
streamlit run app.py

