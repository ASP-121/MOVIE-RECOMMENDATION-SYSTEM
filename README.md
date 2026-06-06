# 🎬 Movie Recommendation System

A **Content-Based Movie Recommendation System** built using **Streamlit**, **scikit-learn**, and **OMDb API**, which recommends movies based on their descriptions. Posters are fetched live using the OMDb API.

Web-link:- https://movie-recommender-system-pawan.streamlit.app/

---

## 🚀 Features

- 🔍 Search and select a movie
- 🎯 Content-based recommendations using TF-IDF + Nearest Neighbors
- 🖼 Automatically fetch movie posters and plots via OMDb API
- 🧠 Uses cosine similarity on TF-IDF vectors
- 📦 Clean and responsive UI built with Streamlit
- 🛡 Graceful handling of missing posters using placeholders

---

## 📊 Demo Screenshot

![App Screenshot](img.jpg)

---

## 🧠 How It Works

- The dataset contains movies and their descriptions.
- The `TfidfVectorizer` converts descriptions into numerical vectors.
- The `NearestNeighbors` model finds the most similar descriptions to the selected movie.
- For each recommended title, the OMDb API provides a poster and plot.
- If the poster is not found, a placeholder is shown.

---

## 🛠 Tech Stack

- [Python](https://www.python.org/)
- [Pandas](https://pandas.pydata.org/)
- [scikit-learn](https://scikit-learn.org/)
- [Streamlit](https://streamlit.io/)
- [OMDb API](https://www.omdbapi.com/)

---

## 📁 Project Structure

    ├── app.py # Main Streamlit app
    ├── img.jpg # Banner image for the UI
    ├── movies_content.csv # Movie dataset with titles and descriptions
    ├── requirements.txt # Python dependencies
      └── README.md # Project documentation
---

## 🔧 Installation

1. **Clone the repository**:

       git clone https://github.com/2000pawan/Content_Based_Movie_Recommendation_System.git
       cd Content_Based_Movie_Recommendation_System
2. Install dependencies:

       pip install -r requirements.txt
       Run the app:
       streamlit run app.py
---

## 🔑 OMDb API Key
You must have a valid OMDb API key.

Replace the default key in app.py:

api_key = "your_omdb_api_key_here"

## 📌 Sample Dataset Format

title	description

Inception	A thief who steals corporate secrets...

The Dark Knight	Batman raises the stakes in his war...

Make sure your CSV has a title and description column.


### 📄 License

This project is licensed under the MIT License.
