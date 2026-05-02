# 📚 Book Recommendation System


A **Machine Learning web application** that recommends books using **Popularity-Based Filtering** and **Collaborative Filtering**.
This system helps users discover books based on overall popularity and personalized similarity between books.

---

## 🚀 Features

* ⭐ Displays top popular books based on ratings
* 🤝 Recommends similar books using collaborative filtering
* 🌐 Interactive web interface using Flask
* 📊 Uses cosine similarity for accurate recommendations
* ⚡ Fast predictions using precomputed `.pkl` model files

---

## 🧠 How It Works

### 1. Popularity-Based Recommendation

* Books are ranked based on:

  * Number of ratings
  * Average rating
* Displays most popular books on the homepage

---

### 2. Collaborative Filtering

* Uses user-item interaction matrix
* Finds similarity between books using cosine similarity
* Recommends top similar books based on user input

---

## 🏗️ Project Structure

```
P2_Book_Recommendation_System/
│
├── app.py
├── README.md
├── requirements.txt
├── .gitignore
│
├── data/
│   ├── Books.csv
│   ├── Ratings.csv
│   └── Users.csv
│
├── model/
│   ├── books.pkl
│   ├── popular.pkl
│   ├── pt.pkl
│   └── similarity_scores.pkl
│
├── notebook/
│   └── P2.ipynb
│
├── templates/
│   ├── index.html
│   └── recommend.html
│
├── static/
│   └── images/
│       ├── classicRec.png
│       ├── DeepRec.png
│       └── recsys_taxonomy2.png
│
└── venv/   (ignored via .gitignore)
```

---

## ⚙️ Tech Stack

* Python 
* Flask 
* Pandas 
* NumPy 
* Scikit-learn 
* Pickle 

---

## 💡 Usage

* Homepage → Shows popular books
* Recommendation Page → Enter a book name to get similar books

---

## 🧾 Code Overview

The main logic is implemented in:


* Loads trained models using `pickle`
* Displays popular books on homepage
* Recommends books using similarity matrix

---

## 📊 Dataset

Uses the **Book-Crossing Dataset**, which includes:

* Book details
* User ratings
* User information
