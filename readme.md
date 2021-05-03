# Spotify Dataset 1922-2021, ~600k Tracks
## by Abdulrahman Yaseen


## relevant and required software.

This project has two parts that demonstrate the importance and value of data visualization techniques in the data analysis process. In the first part, you will use Python visualization libraries to systematically explore a selected dataset, starting from plots of single variables and building up to plots of multiple variables. In the second part, you will produce a short presentation that illustrates interesting properties, trends, and relationships that you discovered in your selected dataset. The primary method of conveying your findings will be through transforming your exploratory visualizations from the first part into polished, explanatory visualizations.

This project uses Python 3 and is designed to be completed through the Jupyter Notebooks IDE. It is highly recommended that you use the Anaconda distribution to install Python, since the distribution includes all necessary Python libraries as well as Jupyter Notebooks. The following libraries are expected to be used in this project:

NumPy
pandas
Matplotlib
Seaborn

## Dataset


Audio features of ~600k songs released in between 1922 and 2021 (A Kaggle Dataset)
There are 586672 tracks in the dataset with 19 features

Numerical:
- acousticness (Ranges from 0 to 1)
- danceability (Ranges from 0 to 1)
- energy (Ranges from 0 to 1)
- duration_ms (Integer typically ranging from 200k to 300k)
- instrumentalness (Ranges from 0 to 1)
- valence (Ranges from 0 to 1)
- popularity (Ranges from 0 to 100)
- tempo (Float typically ranging from 50 to 150)
- liveness (Ranges from 0 to 1)
- loudness (Float typically ranging from -60 to 0)
- speechiness (Ranges from 0 to 1)

Dummy:

- mode (0 = Minor, 1 = Major)
- explicit (0 = No explicit content, 1 = Explicit content)

Categorical:

- key (All keys on octave encoded as values ranging from 0 to 11, starting on C as 0, C# as 1 and so on…)
- timesignature (The predicted timesignature, most typically 4)
- artists (List of artists mentioned)
- artists (Ids of mentioned artists)
- release_date (Date of release mostly in yyyy-mm-dd format, however precision of date may vary)
- name (Name of the song)


## Summary of Findings

> The popularity is right skewed as the popularity is calculated on the total number of plays the track has had and how recent those plays are. So it's reasonable that most of the tracks have a popularity of zero, and zero tracks have a popularity of 100
The durations ranges from 100,000 ms to 500,000 ms with large freq at duration of 200,000 ms (3.3 minutes)
Tracks have become more Energetic and Danceable in the recent years. The loudness and tempo has also increased. The tracks have become less "Acoustic" Also the more energetic and loud the more popular
Valence and Danceability are highly related and so is speechiness and Danceability
Over Years songs are getting louder and the louder the more popular, energitic and the more danceable


## Key Insights for Presentation

> Over Years songs are getting louder and the louder the more popular, energitic and the more danceable

## files included in the project

Spotify_Dataset.ipynb / Spotify_Dataset.html : Contains all exploratory analysis
Spotify_Dataset_Slide.ipynb / Spotify_Dataset_Slide.slides.html : Contains all explanatory analysis
readme.md : readme file
tracks.csv : our data

## Acknowledgements

I would thank to Spotify Developers website for creating a very good documentation for Spotify Web API, Spotipy (Python module for Spotify web servers) for making the requesting process more flexible, and I want to especially thank to Kaggle Community for allowing me the opportunity to share this project!