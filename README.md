# Music Mood Analysis 

The **Music Mood Analysis and Spotify Wrapped Predictor** is a Python-based project designed to analyze users' listening habits and predict their music preferences. By utilizing machine learning models and Spotify's API, the system identifies a user's music mood tendencies and provides insights similar to Spotify Wrapped.


## Key Features

- **Music Mood Prediction**:
  - Analyzes users' liked songs and categorizes them into moods (Happy, Sad, Chill, Energetic).
  - Predicts the mood distribution of a user's music taste using machine learning models.

- **Audio Feature Extraction**:
  - Extracts key audio features from Spotify playlists and user-saved tracks using **Spotipy**.
  - Uses **Essentia** for in-depth rhythm and BPM analysis.

- **Data Processing and Cleaning**:
  - Filters out conflicting moods in duplicated song names.
  - Applies **Z-score normalization** and **Standard Scaling** to prepare data for model training.

- **Machine Learning Classification**:
  - Implements multiple classifiers (Random Forest, Decision Trees, SVM, Neural Networks, etc.).
  - Selects the best-performing model for mood prediction.


## Technologies Used

- **Programming Language**: Python
- **Audio Processing**: Essentia, Pydub
- **Machine Learning**: Scikit-learn, NumPy, Pandas
- **Spotify API**: Spotipy
- **Data Handling**: JSON, CSV


## How It Works

1. **Data Collection**:
   - Retrieves user's liked songs from Spotify.
   - Extracts features from mood-based Spotify playlists.
   
2. **Preprocessing and Feature Engineering**:
   - Drops irrelevant attributes and normalizes data.
   - Handles duplicates and conflicting labels.
   
3. **Model Training & Evaluation**:
   - Trains multiple classifiers and selects the best model using cross-validation.
   
4. **Music Mood Prediction**:
   - Predicts the mood distribution of a user's listening habits.
   - Outputs a percentage breakdown of each mood category.


## Setup Instructions

1. Clone the repository:
   ```sh
   git clone https://github.com/ceasarattar/MusicAnalysis.git
   cd MusicAnalysis
   ```
2. Set up Spotify API credentials in `library.py` and `spotify_mood_playlist.py`.
3. Run the script to analyze music preferences:
   ```sh
   python modeling.py
   ```
