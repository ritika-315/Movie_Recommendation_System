🎬 Movie Recommendation System

This project is a content-based movie recommendation system that suggests similar movies based on a selected movie.
It uses Natural Language Processing (NLP) techniques on movie descriptions and metadata.

The system is built using:

Machine Learning (TF-IDF + Cosine Similarity)

FastAPI for backend

Streamlit for frontend UI

---

✨ Project Features

Recommends movies based on content similarity

Uses movie overview, genres, and tagline

Fast recommendations using TF-IDF Vectorization

REST API using FastAPI

User-friendly interface using Streamlit

Pre-trained model saved using pickle

---

🛠️ Technologies Used

Python

Pandas, NumPy

Scikit-learn

FastAPI

Uvicorn

Streamlit

---

📊 Dataset Description

The dataset contains movie metadata such as:

Title

Overview

Genres

Tagline

Popularity

Vote Average

These features are combined and cleaned to create a tags column, which is used for generating recommendations.

---

⚙️ How the Recommendation Works

Combine important text features into one column

Convert text into numerical form using TF-IDF

Calculate similarity using Cosine Similarity

Recommend top N similar movies based on similarity score

---

▶️ How to Run the Project Locally
Step 1: Clone the repository
git clone https://github.com/your-username/Movie_Recommendation_System.git
cd Movie_Recommendation_System

Step 2: Create and activate virtual environment (Windows)
python -m venv .venv
.\.venv\Scripts\Activate.ps1

Step 3: Install required packages
pip install -r requirements.txt

Step 4: Start FastAPI backend
uvicorn main:app --reload


Backend will run at:

http://127.0.0.1:8000


API documentation:

http://127.0.0.1:8000/docs

Step 5: Start Streamlit frontend
streamlit run app.py


Frontend will open at:

http://localhost:8501

🔌 API Usage Example

Endpoint: /recommend

Parameters:

title = movie name
n = number of recommendations


Response Example:

{
  "recommended_movies": [
    "Interstellar",
    "The Prestige",
    "Shutter Island"
  ]
}

---

🎯 Example

Input Movie:

Inception

Recommended Movies:

Interstellar
The Dark Knight
The Prestige
Shutter Island

---

🚀 Future Enhancements

Add collaborative filtering

Display movie posters using TMDB API

Improve ranking using ratings

Deploy on Render or AWS

Add user login system
