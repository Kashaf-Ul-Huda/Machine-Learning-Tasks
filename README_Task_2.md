# 🎬 Movie Recommendation System

This project is part of my internship program at **Elevvo Pathways**.  
It implements a **Movie Recommendation System** using **Collaborative Filtering** approaches on the **MovieLens 100K dataset**.  

---

## 📌 Project Overview
Recommender systems are at the core of platforms like Netflix, YouTube, and Spotify.  
In this project, we built and compared two popular approaches:
- **Item-based Collaborative Filtering**
- **Matrix Factorization using SVD (Singular Value Decomposition)**

Our goal was to recommend movies to users based on their previous ratings and behavior patterns.

---

## 📂 Dataset
We used the [MovieLens 100K dataset](https://grouplens.org/datasets/movielens/100k/),  
which contains **100,000 ratings** from **943 users** on **1682 movies**.

- **Ratings:** Scale of 1–5
- **Files used:** `u.data`, `u.item`

---

## ⚙️ Methodology
1. **Data Preprocessing**
   - Loaded ratings and movies
   - Merged into a user–item matrix

2. **Item-based Collaborative Filtering**
   - Calculated cosine similarity between movies
   - Recommended movies based on most similar items

3. **Matrix Factorization (SVD)**
   - Used `Surprise` library to implement SVD
   - Trained and evaluated on 80/20 split

4. **Evaluation Metrics**
   - Root Mean Squared Error (RMSE)
   - Precision@K & Recall@K (optional, but sparse results)

---

## 📊 Results
| Method      | RMSE   |
|-------------|--------|
| Item-based  | 0.9756 |
| SVD         | 0.9376 |

✅ **SVD outperformed Item-based filtering**, providing more accurate rating predictions.  
Hence, SVD was chosen for deployment.

---

## 🚀 Deployment
We built a simple **Gradio app** for demo purposes:  
- User enters a **User ID**
- System returns top movie recommendations from:
  - **Item-based Filtering**
  - **SVD**

This allows easy side-by-side comparison.

---

## 🛠️ Tech Stack
- **Python 3**
- **Libraries:** Pandas, NumPy, Scikit-learn, Surprise, Gradio, Matplotlib
- **Platform:** Google Colab

---

## 📌 Future Improvements
- Add **Hybrid filtering** (combine content + collaborative)
- Deploy as a **web service** (Flask/FastAPI + frontend)
- Enhance evaluation with larger datasets (MovieLens 1M, 10M)

---

## 👩‍💻 Author
**Kashaf Ul Huda**  
AI/ML Intern @ Elevvo Pathways  
Passionate about AI, NLP, and Computer Vision 🚀  
