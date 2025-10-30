# 🎧 Yes We Jam – A Music Recommendation System

A data-driven exploration and machine learning project that builds a music recommendation system using Spotify data. Inspired by Barack Obama's playlists (2019-2024), the project investigates what makes a song likely to appear on a curated playlist like his.

---

## 📌 Project Summary

This project analyzes Spotify tracks through data collection, enrichment, statistical testing, and machine learning to:
- Explore musical trends across genres and playlists
- Predict whether a song fits Obama's playlists
- Recommend similar tracks

---

## 🔍 Key Features

- ✅ Data collection via Spotify API (track & artist-level)
- 📊 Statistical testing (Shapiro, t-test, Mann–Whitney U)
- 🤖 Machine learning (Random Forest, KNN, Logistic Regression)
- 🔮 Playlist prediction using sigmoid probability
- 📈 Exploratory analysis, correlation heatmaps, and visual storytelling

---

## 🛠 Tools & Technologies

| Tool           | Use Case                             |
|----------------|--------------------------------------|
| `Python`       | Core development                     |
| `pandas`       | Data manipulation                    |
| `matplotlib`, `seaborn` | Visualizations               |
| `scipy.stats`  | Statistical analysis                 |
| `sklearn`      | Machine learning models              |
| `Spotify API`  | Track & artist metadata              |
| `BigQuery`     | Cloud data storage & export          |
| `Git & GitHub` | Version control & collaboration      |

---

## 🧠 Notebooks Overview

| Notebook                                   | Description                                                |
|-------------------------------------------|------------------------------------------------------------|
| `get_multiple_artist_info_from_Spotify_API.ipynb` | Retrieves track & artist data via Spotify API        |
| `MRS_statistical_testing.ipynb`           | Tests distributions, compares Obama Playlists vs. Top 100 tracks     |
| `random_forrest.ipynb`                    | Feature importance analysis via Random Forest              |
| `Logistic_regression_Obama_Final.ipynb`   | Predicts song inclusion using logistic regression          |
| `KNN_Model_30k_Spotify_Songs.ipynb`       | Recommends similar tracks using K-Nearest Neighbors (KNN) on 30k Spotify Songs |
| `Obama_vs_Top_100_Comparison.ipynb`       | Visual & numerical comparison of playlist differences      |
| `cat_var_training_testing_list.ipynb`     | Prepares categorical variables for ML pipeline             |
| `big_query_template.ipynb`                | Data export to Google BigQuery                             |

---

## 💡 Insights

- Obama’s playlists favor jazz, soul, and socially conscious lyrics. It was interesting to see how consistent Obama’s music taste remained, with distinct differences in genre, musical features and popularity compared to mainstream tracks
- the differences in artist and track popularity between the 2 datasets, suggest the former President enjoys discovering hidden gems, his playlists include no fewer than 13 "unpopular tracks" with a score of 0, some even by renowned artists
- Key features influencing playlist inclusion: **danceability, valence, and energy**.
- Logistic Regression successfully predicted songs with high playlist fit.

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Ramonalyst/Music_Recommendation_System.git
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
3. Run notebooks in Jupyter or VS Code

## 📁 Data Sources

- [Spotify Web API](https://developer.spotify.com/documentation/web-api)
- Kaggle dataset:
  - [30k Spotify Songs](https://www.kaggle.com/datasets/joebeachcapital/30000-spotify-songs)

### 📁 Data Files Included

This repository includes curated datasets to ensure smooth reproducibility and experimentation:

| Filename | Description |
|---------|-------------|
| `data/30K_spotify_songs_cleaned_V1.csv` | Cleaned version of the Kaggle 30k Spotify dataset
| `data/BO_playlist_2019_2024_artist_enriched.csv` | Barack Obama's curated playlists (2019–2024), enriched with artist-level Spotify metadata. Collected via Spotify API. |
| `data/2024_spotify_top_100_artist_enriched.csv` | Spotify Top 100 songs (2024 edition), enriched with artist-level data for comparative analysis. |
| `data/song_list_obama_wo_duplicates_view.csv` | Clean and unique dataset with consolidated genre categories and no duplicate songs used for genre harmonization and merging. |
 

## 🙋‍♀️ Author

[@Ramonalyst](https://github.com/Ramonalyst)
Data Analyst · Music Enthusiast · Project Lead

## 📬 Connect via LinkedIn

Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/ramona-mufi%C4%87-69b29b281/) for questions, feedback, or collaboration ideas.
Feel free to ⭐ star this repo if you find it useful!

## 🤝 Collaborators

This project was created with the help and collaboration of:
- [MarieGdH](https://github.com/MarieGdH)
- [MISTYCROWHEART](https://github.com/MISTYCROWHEART)

## 📌 License

MIT License – feel free to fork and build on it, just give credit 💙

