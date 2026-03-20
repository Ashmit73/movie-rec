# 🎬 Movie Recommendation System

An intelligent movie recommender system using TF-IDF Content-Based 
Filtering and Genre-Based recommendations powered by TMDB API.

---

##  How It Works

- **TF-IDF Content-Based Filtering** — Movie metadata ke basis pe 
  cosine similarity se similar movies recommend karta hai
- **Genre-Based Filtering** — TMDB API se same genre ki 
  popular movies suggest karta hai

---

## Architecture
```
Streamlit UI (app.py)
      ↓
FastAPI Backend (main.py)
      ↓
TF-IDF Matrix (Scikit-learn)  +  TMDB API
      ↓
Movie Recommendations
```

---

## 🛠️ Tech Stack

| Category | Tools |
|---|---|
| Language | Python 3.10 |
| Backend API | FastAPI, Uvicorn |
| Frontend UI | Streamlit |
| ML | Scikit-Learn, TF-IDF, NumPy, SciPy |
| Data | Pandas, movies_metadata.csv |
| External API | TMDB API (posters & movie details) |
| HTTP Client | HTTPX |
| Deployment | Render (Backend) + Streamlit |

---

## ⚙️ How to Run Locally
```bash
# 1. Clone the repo
git clone https://github.com/Ashmit73/movie-rec
cd movie-rec

# 2. Install dependencies
pip install -r requirements.txt

# 3. Add TMDB API Key in .env
TMDB_API_KEY=your_tmdb_api_key_here

# 4. Start FastAPI backend
uvicorn main:app --reload

# 5. Start Streamlit frontend
streamlit run app.py
```

---

## 📸 Features

- 🔍 Search any movie by keyword
- 🎯 TF-IDF based similar movie recommendations
- 🎭 Genre-based movie suggestions via TMDB
- 🖼️ Movie posters & details from TMDB API
- 📱 Clean responsive Streamlit UI
- ☁️ Backend deployed on Render

---

## 👨‍💻 Author
**Ashmit Agrawal**
[![GitHub](https://img.shields.io/badge/GitHub-Ashmit73-black?style=flat&logo=github)](https://github.com/Ashmit73)
