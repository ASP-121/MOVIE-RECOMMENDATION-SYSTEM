# 🎬 Movie Recommendation System

A **Content-Based Movie Recommendation System** built using **Streamlit**, **scikit-learn**, and **OMDb API**, which recommends movies based on their descriptions. The application features **similarity scoring**, **customizable Top-N recommendations**, and dynamically fetches movie posters and metadata from the OMDb API.

Web-link:- https://movie-recommender-system-pawan.streamlit.app/

---

## 🚀 Features

- 🔍 Search and select a movie
- 🎯 Content-based recommendations using TF-IDF + Nearest Neighbors
- 📊 Displays similarity scores for recommended movies
- 🎚 Customizable Top-N recommendation slider
- ⭐ Displays IMDb ratings
- 📅 Displays release year
- ⏱ Displays movie runtime
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
- Similarity scores are calculated and displayed for each recommendation.
- The OMDb API provides movie posters, IMDb ratings, release year, and runtime.
- If the poster is not found, a placeholder image is shown.

---

## 🛠 Tech Stack

- Python
- Pandas
- NumPy
- scikit-learn
- Streamlit
- Requests
- Pillow (PIL)
- OMDb API

---

## 📁 Project Structure

```
├── app.py                  # Main Streamlit app
├── img.jpg                 # Banner image for the UI
├── movies_content.csv      # Movie dataset with titles and descriptions
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation
```

---

## 🔧 Installation

1. **Clone the repository**:

```bash
git clone https://github.com/ASP-121/MOVIE-RECOMMENDATION-SYSTEM.git
cd MOVIE-RECOMMENDATION-SYSTEM
```

2. **Install dependencies**:

```bash
pip install -r requirements.txt
```

3. **Run the application**:

```bash
streamlit run app.py
```

---

## 🔑 OMDb API Key

You must have a valid OMDb API key.

Create a `.streamlit/secrets.toml` file:

```toml
OMDB_API_KEY = "your_omdb_api_key_here"
```

---

## 📌 Sample Dataset Format

| name | description |
|--------|-------------|
| Inception | A thief who steals corporate secrets through dream-sharing technology. |
| The Dark Knight | Batman raises the stakes in his war on crime. |

Make sure your CSV contains at least the following columns:

- `name`
- `description`

---

## 📈 Future Improvements

- User authentication
- Hybrid recommendation system
- Genre-based filtering
- Watchlist functionality
- Collaborative filtering
- Recommendation explanation dashboard

---

### 📄 License

This project is licensed under the MIT License.
