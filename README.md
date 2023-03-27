# Niyo_Bootcamp_Final_Project_Spotify_Dataset

Project consists of 7 files: The 2 Original dataset (CSV), SQL (Big Query), Excel, Python (Google Colab), PowerBi and the final Powerpoint presentation.

The Original Datasets are from Kaggle and are the ['Spotify Top 10000 Streamed Songs'](https://www.kaggle.com/datasets/rakkesharv/spotify-top-10000-streamed-songs?datasetId=2777839&sortBy=dateCreated&sort=most-comments) and ['Spotify top chart songs 2022'](https://www.kaggle.com/datasets/sveta151/spotify-top-chart-songs-2022) . These datasets are scrapped from the largest streaming software - Spotify, and will be used to see who the top streamed artists were and if factors such as danceability or energy affect the streaming position of the artist. The columns that I am interested in are 'Position, Artist_Name, Song_Name, Peak_Position, weeks_on_chart, Total_Streams, Top_10__xTimes_, danceability, energy, key, loudness, mode, speechiness, acousticness, instrumentalness, liveness, tempo, duration_ms'.

The Presentation will explain the background and my objectives of this project.

## PowerPoint Presentation
What the dataset is about:
My objectives
The preswentation will cover a range of different visuals which will work together to give insigh on the data and help me build the reccommendations at the end.

## SQL

Using BigQuery, I retrieved the dataset and wanted to answer my 3 objectives.

The bigQuery had to be copied to a word document as it cannot be dowloaded directly to Github.

Using a range of statements such as SELECT, FROM, LIMIT, GROUP BY, SUM, ORDER BY, WHERE, BETWEEN, CASE WHEN AND INNER JOIN, I was able to answer the following questions:
1. What are the top 10 most streamed songs?
2. What is TWICE's Current ranking?
3. Is there any information on similar groups to TWICE that may be helpful?
4. What factors obviously show an impact on the number of streams? e.g. number of days the song has been released
5. Are there any null values in the Data, is it necessary to remove them?
6. Does the shape of the data have any impact on the ability to visualise it?

The general insights that I recieved from this SQL query was that:
Drake was the most streamed artist, but the most streamed song was Sunflower: Spider Man by Post Malone.
The highest rank that Twice had gained was 83rd, but a similar group, BTS, had songs that had peaked at 1st. Duration had an impact on the total streams, longer the song has been released, the more streams it is likely to have.

Also, CASE WHEN showed that the majority of the Data was within 'less than 100million streams', which suggested that the data set would have to be split to get clearer visuals.

## Excel
Using SUM, MAX and XLOOKUP i was able to note what song had been in the top 10 the most number of times (Sunflower: spiderman) which would be useful later in the analysis.

There is a total of 200 billion streams (from the songs) and Sunflower Spiderman accounts for 0.4% of this number. It also has been in the top 10 302 times, which is higher than the other songs.

## Python
Realised that may have to split the data into top and bottom half of positions. 



## PowerBI


