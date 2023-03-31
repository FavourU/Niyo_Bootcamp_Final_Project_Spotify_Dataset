# Niyo Bootcamp Final Project: Spotify EDA

Project consists of 9 files: The README, The 2 Original dataset (CSV), A merged dataset (from python), SQL (Big Query), Excel, Python (Google Colab), PowerBi and the final Powerpoint presentation.

The Original Datasets are from Kaggle and are the ['Spotify Top 10000 Streamed Songs'](https://www.kaggle.com/datasets/rakkesharv/spotify-top-10000-streamed-songs?datasetId=2777839&sortBy=dateCreated&sort=most-comments) and ['Spotify top chart songs 2022'](https://www.kaggle.com/datasets/sveta151/spotify-top-chart-songs-2022) . These datasets are scrapped from the largest streaming software - Spotify, and will be used to see what the top streamed songs are and if factors such as danceability or acousticness affect the streaming position of the artist.

The Presentation will explain the background and my objectives of this project.

## PowerPoint Presentation

Titled : Presentation on Spotify EDA Project

This Powerpoint will cover some insights I gained from the datasets using SQL, Python, PowerBi and Excel. I will apply the data to try and solve a business questions in relation to TWICE who are a Kpop girls group. In trying to understand what causes songs to rank in the top 10, i will also observe ways that TWICE can increase their streaming numbers, as well as realistic goals that they should set for themselves.

#My objectives:
1. What are the top 10 songs
2. What factors contribute to streaming number?
3. What recommendations would be useful to TWICE so that their song can reach top 10?

The presentation will cover a range of different visuals which will work together to give insigh on the data and help me build the reccommendations at the end.

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
After importing the necessary dataframes, i merged the dataframes together based on the artist name and song name. After cleaning up the dataframe, i removed rows that i deemed were unecessary. As my project objective was focusing on how to get within the top 10, i thought it unneccessary to have datapoints that are not within top 10, so removed thos using loc.

Used Python to visualise some of the data and derive insights from it.


## PowerBI

To create the dashboard, I had to import a specific dataframe from my python (specific to songs within top 10). Looking at the Duration, Properties (Danceability, energy, acousticness, speechiness) and release days of the song will allow for recommendations to be made to improve the streaming number of TWICE.

The python section required me to use 3 different tables, Unpivot certain columns (danceability, energy, acousticenss and speechiness) and do calculations to convert milliseconds into seconds to make the graph more readable.

I chose a dark theme to fit with the presentation and the overall theme of the Project.

