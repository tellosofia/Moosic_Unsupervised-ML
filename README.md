# Case Study: Automating Playlist Creation for Moosic

## Welcome to Moosic!

Moosic is a start-up dedicated to creating playlists curated by music experts, blending old and new trends. Users can subscribe to it's website and listen to these playlists through their preferred music app (Spotify, Apple Music, YouTube Music, etc.). Moosic's playlists are known for their personal touch, encapsulating distinct "moods" and "styles."

## Objectives

The primary goal of this project is to:
- Use a dataset collected from the Spotify API containing audio features (tempo, energy, danceability, etc.) for thousands of songs.
- Apply a basic clustering algorithm, K-Means, to divide the dataset into clusters, which will form the basis of new playlists.

Key questions include:
- Are Spotify’s audio features effective in identifying “similar songs” as defined by human criteria?
- Is K-Means a suitable method for creating playlists, or should other methods be explored?

## Project Overview

### Understanding Audio Features
The data used to group songs are Spotify’s audio features. The playlists emerging from the clustering algorithm will be determined by the information these audio features capture. It's important to understand these features and relate them to human perceptions of music.

### Key Spotify Audio Features
- **Acousticness**: Confidence measure of whether the track is acoustic.
- **Danceability**: Describes how suitable a track is for dancing.
- **Duration**: The duration of the track in milliseconds.
- **Energy**: Perceptual measure of intensity and activity.
- **Instrumentalness**: Predicts whether a track contains no vocals.
- **Key**: The key the track is in, using standard Pitch Class notation.
- **Liveness**: Detects the presence of an audience in the recording.
- **Loudness**: The overall loudness of a track in decibels.
- **Mode**: Indicates the modality (major or minor) of a track.
- **Speechiness**: Detects the presence of spoken words in a track.
- **Tempo**: The overall estimated tempo of a track in beats per minute.
- **Time Signature**: The estimated overall time signature of a track.
- **Valence**: Describes the musical positiveness conveyed by a track.

## Methodology

1. **Data Collection**: Gather audio features from the Spotify API for a large dataset of songs.
2. **Data Processing**: Clean and preprocess the data for analysis.
3. **Clustering**: Apply K-Means clustering to group songs into playlists based on their audio features.
4. **Evaluation**: Assess the quality of the clusters by comparing them to human-judged similarities between songs.
5. **Iteration**: Refine the model based on feedback and further analysis.

## Tools and Technologies

- **Programming Language**: Python
- **Data Collection**: Spotify API
- **Data Processing**: Pandas, NumPy
- **Clustering Algorithm**: Scikit-learn (K-Means)
- **Visualization**: Matplotlib, Seaborn
- **Notebook Environment**: Jupyter Notebooks

## Expected Outcomes

The project will result in an initial prototype of automated playlists created using K-Means clustering. We will evaluate the effectiveness of Spotify’s audio features in grouping similar songs and determine whether K-Means is a suitable method for this task.

