# Niyo_Bootcamp_Final_Project_Spotify_Dataset

Project consists of 7 files: The 2 Original dataset (CSV), SQL (Big Query), Excel, Python (Google Colab), PowerBi and the final Powerpoint presentation.

The Original Datasets are from Kaggle and are the ['Spotify Top 10000 Streamed Songs'](https://www.kaggle.com/datasets/rakkesharv/spotify-top-10000-streamed-songs?datasetId=2777839&sortBy=dateCreated&sort=most-comments) and ['Spotify top chart songs 2022'](https://www.kaggle.com/datasets/sveta151/spotify-top-chart-songs-2022) . These datasets are scrapped from the largest streaming software - Spotify, and will be used to see who the top streamed artists were and if factors such as danceability or energy affect the streaming position of the artist. The columns that I am interested in are 'Position, Artist_Name, Song_Name, Peak_Position, weeks_on_chart, Total_Streams, Top_10__xTimes_, danceability, energy, key, loudness, mode, speechiness, acousticness, instrumentalness, liveness, tempo, duration_ms'.

## SQL

Using BigQuery, I retrieved the dataset and wanted to answer my 5 basic question (covered in Powerpoint presentation)

Method:
1. SELECT, FROM, LIMIT were used to retrieve the top 100 rows from the analysis
2. The ''Spotify Top 10000 Streamed Songs' was saved as 'Analysis' table, and the 'Spotify top chart songs 2022' was saved as 'Short' table
3. GROUP BY, SUM and ORDER BY were used to find the top 10 most streamed artists. Some artists had multiple songs in the top 10,000 and so it was necessary to find the total streams of the songs and group the artist to find out the overall top streamed artist.
4. Comparing BTS in the Dataset (using >WHERE Artist_Name LIKE '%BTS%') to the current number of streams made me question why their popularity skyrocketed, compared to some of the other artists such as Post Malone. The second Dataset, looking at Danceability etc, may give more of an insight on why this happens. Dataset actually showed that BTS songs have been in the top 10000 more times than Post Malone songs, even though Post Malone is the 2nd most streamed and BTS is the 101st most streamed.
5. Using 'WHERE Days BETWEEN 0 AND 20' hinted towards a relationship between Number of days that a song has been released, and the position in top 10000.
6. Looked for Null values in Song name, found 4 but decided to keep them in, incase they were useful in my analysis
7. Realised that as many artists only had 1 song in the top 10,000, when looking for the average number of times in top 10, the results where sweked because of this.
8. To see the total streams, in buckets, and have an idea of the distribution, used CASE WHEN and found that most of the songs had total streams les than 100 million. I suggest that the data be split as certain results are skewing the data, which mmay make it difficult to visualise well.

## Excel

Much like SQL, i used Excel functions such as ... to find out the 

## Python
Realised that may have to split the data into top and bottom half of positions. 



## PowerBI

## PowerPoint Presentation
