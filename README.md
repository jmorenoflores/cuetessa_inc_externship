# Project: **Predicting Valence Score of Songs with Machine Learning**

## Description and Purpose of Project:

This project aimed to develop a Machine Learning Model that predicts the valence score of songs utilizing features from the songs' spectograms, such as tempo (beat per minute value only), spectral centroids, spectral rolloffs, spectral contrast - 7 bands, mel frequency coefficients - 20 coefficients, zero crossing rate, chroma energy normalized statistics - 12 chromas, root mean squared error, spectral influx (mean and variance of Numpy array only), and onset rate. Similarly, we also acquired meta data from the Spotify for Developers API and used them as features including: danceability, energy, key, loudness, mode, speechiness, acousticness, instrumentalness, liveness, duration_ms, time_signature. 

## Business value:

The ultimate goal of the project is to enhance the music listening experience for Cuetessa, Inc's users by accurately assigning songs to appropriate playlists based on their valence scores.


The following table of contents the structure used in this project:
```
1. Project for Cuetessa, INC: Predicting Valence Score of Songs
1.1 Data Preprocessing

1.1.1 Describing the data
1.1.2. Data types and missing values
1.1.2.1 song_name column 
1.1.2.2 song_id column 
1.1.2.3 song_preview_url column 
1.1.2.4 artist_name column 
1.1.2.5 artist_uri column 
1.1.2.6 danceability column 
1.1.2.7 energy column 
1.1.2.8 Key column 
1.1.2.9 Loudness column 
1.1.2.10 Mode column 
1.1.2.11 Speechiness column 
1.1.2.12 accousticness column 
1.1.2.13 instrumentalness column 
1.1.2.14 liveness column 
1.1.2.15 valence column 
1.1.2.16 valence column 
1.1.2.17 duration_ms column 
1.1.2.18 time_signature column 
1.1.2.18 The following columns: all_sp_centroids, all_rolloffs, all_spectral_costrast, all_mfcc, all_zrs, all_chromas, all_influx, all_onset_rate, and all_rmse were deleted because there was an error while saving numerical data in the columns. Therefore, the data was collected on spectral centroids, spectral rolloffs, spectral contrast, Mel Frequency Cepstral Coefficients, zero crossing rates, chroma energy normalized statistics, spectral influx, onset rates, and root mean square error values from .wav files of the songs.
1.1.2.18 spectral centroids columns
1.1.2.19 spectral rolloffs columns
1.1.2.20 spectral contrast columns
1.1.2.21 zero crossings columns
1.1.2.21 spectral influx columns
1.1.2.22 Mel Frequency coefficient statistics columns
1.1.2.23 RMSE columns
1.1.2.23 onset_rate columns
1.1.2.24 Chroma Energy Normalized Statistics (CENS) columns
1.1.2.25 Deleting columns
1.2 Exploratory Data Analysis
1.2.1 Histogram and Violinplot of Valence Scores
1.2.2 Scatter Matrix and correlation coefficients of Meta data
1.2.3 Top 10 Songs with Highest Valence Scores from Data
1.2.3 Top 10 Songs with Lowest Valence Scores from Data
1.2.4 Pivot Table 1: Top 10 Artists with Highest Valence Scores, On Average
1.2.5 Pivot table 2: Top 10 Artists with the Lowest Valence Score, On Average

1.3 Model Training
1.3.1 Model 0: Linear Regression Model
1.3.1b Model 0b: Linear Regression Model, without Meta Data
1.3.1c Model 1c: Linear Regression Model, Meta Data Only
1.3.1d Model 0d: Linear Regression Model, Nomalized Features
1.3.2 Model_1 RandomForestRegressor Model
1.3.2b Model_1b RandomForestRegressor Model, Without Meta Data
1.3.2c Model 1c Random Forest Regressor, Only Meta Data
1.3.2d Model 1d Random Forest Regressor, Normalized Features
1.3.3 Model_2 XGBoostRegressor Model
1.3.3b Model 2b XGBoostRegressor Model, Without Meta Data
1.3.3c Model 2c XGBoostRegressor Model, Meta Data Only
1.3.3d Model 2d XGBoostRegressor Model, Normalized Features
1.3.4 Model_3 Support Vector Regressor
1.3.4b Model 3b Support Vector Regressor Model, Without Meta Data
1.3.4c Model 3c Support Vector Regressor, Meta Data Only
1.3.4d Model 3d Support Vector Regressor, Normalized Features
1.3.5 Model_4 K-Nearest Neighbors
1.3.5b Model 4b K-Nearest Neighbor, Without Meta Data
1.3.5c Model 4c K-Nearest Neightbors, Meta Data Only
1.3.5d Model 4d K-Nearest Neighbors, Normalized Features

1.4 Selecting Best Model for Testing

1.5 Conclusion

```

## Tools and concepts used in project:
- pandas
- spotipy 
- SpotifyClientCredentials
- seaborn
- librosa
- librosa.display
- minmax_scale
- matplotlib.pyplot
- numpy
- LinearRegression
- import train_test_split
- GridSearchCV
- RandomizedSearchCV
- mean_squared_error
- mean_absolute_error
- math
- SVR
- RandomForestRegressor
- xgboost
- KNeighborsRegressor
- StandardScaler

