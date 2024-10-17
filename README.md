# Spotify Music Analysis and Recommendation System

This project aims to explore the Spotify dataset and use various machine learning techniques for data analysis, clustering, and building a song recommendation system. It involves visualizing the characteristics of different songs and genres, understanding how music evolved over time, and applying clustering algorithms like K-Means to group songs and genres based on audio features.

## Project Overview

### 1. **Import Libraries**

We begin by importing essential Python libraries for data manipulation, visualization, and machine learning. This includes popular libraries such as Pandas, NumPy, Seaborn, Matplotlib, and Scikit-learn.

### 2. **Dataset**

The project uses three main datasets:
- `data.csv`: Contains audio features and popularity metrics of various songs.
- `data_by_genres.csv`: Grouped by genres, this dataset provides aggregate audio features.
- `data_by_year.csv`: Aggregated audio features by year to analyze music trends over time.

### 3. **Exploratory Data Analysis (EDA)**

Several visualizations are created to understand the data:
- **Music Over Time**: Analyzing how music has changed from 1921 to 2020 using features like acousticness, danceability, energy, and more.
- **Characteristics of Different Genres**: Comparing audio features across different music genres.

### 4. **Clustering with K-Means**

We use K-Means clustering to:
- **Cluster Genres**: Genres are grouped into 10 clusters based on their audio features.
- **Cluster Songs**: Songs are grouped into 20 clusters. Visualization of these clusters is done using PCA and t-SNE for dimensionality reduction.

### 5. **Building a Music Recommendation System**

A content-based recommendation system is built using the clusters and audio features. The system recommends similar songs based on the input songs using the Spotipy library to fetch song data from Spotify.

## Key Features

- **Data Analysis**: Visualizations created using Matplotlib, Seaborn, and Plotly to understand trends in music over time and across genres.
- **K-Means Clustering**: Implementation of K-Means to group songs and genres into clusters based on audio features.
- **Song Recommendation System**: A content-based recommendation system that suggests songs similar to the ones provided by the user.

## Installation

To run the project, you need to install the required libraries. You can install the dependencies using pip:

```bash
pip install -r requirements.txt
```

The project uses the following libraries:
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Plotly
- Scikit-learn
- Spotipy

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/moazzam3214/spotify-music-analysis.git
   cd spotify-music-analysis
   ```

2. Ensure you have created a Spotify app and have your `SPOTIFY_CLIENT_ID` and `SPOTIFY_CLIENT_SECRET`. Add these to your environment variables or configure them in your code.

3. Run the Jupyter notebook to explore the data, analyze genres and songs, and build the music recommendation system.

## Example

```python
recommend_songs([{'name': 'Come As You Are', 'year': 1991},
                 {'name': 'Smells Like Teen Spirit', 'year': 1991}], data)
```

## Visualizations

- **Music Over Time**: A line graph showing the changes in audio features of songs over time.
- **Genres and Clusters**: Bar charts and scatter plots of genres and song clusters using t-SNE and PCA.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
