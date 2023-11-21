# Spotify-Music-Machine-Learning
## Using LDA, QDA, SVM, K-means, and XGBoost on Spotify's Most Popular Songs

In the following project I utilize Linear Discriminant Analysis (LDA), Quadratic Discriminant Analysis
(QDA), and Support Vector Machines (SVM) techniques for classification. I then use K-means clustering and finally build a gradient bosoting model using XGBoost.

I will be using a dataset of songs collected using the Spotify API from the Kaggle at this link:
https://www.kaggle.com/datasets/purumalgi/music-genre-classification/data. The data was originally
collected for MachineHack Hackathon. It contains 17,996 rows with 17 columns. 
The following predictor variables are available:
* artist_name: Name of the artist (String)
* track_name: Name of the song (String)
* popularity: Popularity of the Song (float from 0 to 100)
* danceability: Whether the song is danceable or not (float from 0 to 1)
* energy: What is the energy level of the song (float from 0 to 1)
* key: The Key of the song is represented by an int for the note (integer from 1 to 11)
* loudness: What is the loudness of the music in Db (float from -inf to inf)
* mode: (int either 0 or 1)
* speechiness: amount of vocals in the song (float from 0 to 1)
* acousticness: A measure of how acoustic a song is. Songs with higher acousticness are more likely to use non-electronic instruments. (float from 0 to 1)
* instrumentalness: A measure of how likely it is that a song contains no vocals (float from 0 to 1)
* liveness: value describes the probability that the song was recorded live (float from 0 to 1)
* valence: Describes the musical positiveness conveyed by the song (float from 0 to 1)
* tempo: The overall estimated tempo of a track in beats per minute (int from 0 to inf)
* duration In milliseconds: How long is the song (float from 0 to inf)
* time_signature: Number that indicates how many counts are in each measure (Integer greater than 0)

It has one target variable, named class, with 11 classes representing the song belonging to one of the following. The Genres are ordered from 0 to 10:

* Rock 
* Indie 
* Alt 
* Pop 
* Metal 
* HipHop 
* Alt_Music
* Blues
* Acoustic/Folk
* Instrumental
* Country
