# FUTURE_DS_01

# Spotify Most Streamed Songs: Data Cleaning and Exploratory Data Analysis (EDA)

## Technologies Used

- **Python**: Data cleaning and analysis
- **Pandas**: Data manipulation
- **Seaborn & Matplotlib**: Data visualization
- **Jupyter Notebooks**: Interactive analysis and visualizations

## Project Overview

This project focuses on data cleaning and exploratory data analysis of Spotify's most-streamed songs. The primary objective is to preprocess and analyze song data to uncover trends, patterns, and insights regarding popular music attributes, artist popularity, and streaming behaviors.

## Dataset

The dataset contains information on Spotify’s most-streamed songs, with features like:
- **Track Name**
- **Artist Name(s)**
- **Streams** (number of streams per track)
- **Release Date** (year, month, day)
- **Audio Features**: BPM, key, mode, danceability, energy, valence, etc.
- **Playlist and Chart Presence**: Presence in Spotify, Apple, and Deezer playlists and charts

The dataset may contain inconsistencies, missing values, and non-numeric formatting, making data cleaning a crucial first step.

## Project Workflow

### 1. Data Cleaning

- **Converting Data Types**: Ensured all numeric entries are in their correct format for analysis
- **Handling Missing Values**: Impute entries with missing values using the median since it was the most appropriate in this case.
- **Standardizing Columns**: Ensuring consistency in column names and formats.
- **Date Parsing**: Combined and convert `released_year`, `released_month`, and `released_day` columns into a single `released_date` column as a `datetime` object.
- **Feature Engineering**: Create additional relevant features, such as the **song age** from the release date.

### 2. Exploratory Data Analysis (EDA)

- **Distribution Analysis**: Analyzed distributions of key features, such as streams, danceability, energy, and acousticness.
- **Top Artists Analysis**: Identified the most popular artists by total streams and song count.
- **Trend Analysis**: Explored how popular song attributes (e.g., energy, danceability) have changed over time.
- **Correlation Analysis**: Identifed relationships between different audio features (e.g., energy vs. acousticness).
- **Right-Skewness**: Visualized and addressed the right-skewed distribution of streams.
  
### 3. Visualization

I used these visualization libraries Matplotlib and Seaborn, visualizations include:
- Histograms and KDE plots for feature distributions
- Scatter plots and pair plots for feature relationships
- Line charts for trend analysis over time
- Heatmaps for correlation analysis among features

## Key Insights

1. **Most Streamed Artists**: The Weeknd, Taylor Swift, Ed Sheeran, Harry Styles, Bad Bunny
2. **Popular Song Attributes**: Dominance of negative mood over time
3. **Trends Over Time**: Reduction in acousticness but increase in danceability and energy over time
4. **Streaming Patterns**: Right-skewed distribution indicating a small number of hit songs with very high streams.

## Conclusion

This analysis provides insights into factors that may contribute to a song's popularity on Spotify. Future work could involve building predictive models based on song attributes to estimate potential streaming success.

## License

This project is open-source under the MIT License.
