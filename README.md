# Niyo Bootcamp Final Project: Spotify EDA

Project consists of 9 files: The README, The 2 Original dataset (CSV), A merged dataset (from python), SQL (Big Query), Excel, Python (Google Colab), PowerBi and the final Powerpoint presentation.

The Original Datasets are from Kaggle and are the ['Spotify Top 10000 Streamed Songs'](https://www.kaggle.com/datasets/rakkesharv/spotify-top-10000-streamed-songs?datasetId=2777839&sortBy=dateCreated&sort=most-comments) and ['Spotify top chart songs 2022'](https://www.kaggle.com/datasets/sveta151/spotify-top-chart-songs-2022) . These datasets are scrapped from the largest streaming software - Spotify, and will be used to see what the top streamed songs are, and if factors such as danceability or acousticness affect the streaming position of the song.

The Presentation will explain the background and my objectives of this project.

## PowerPoint Presentation

Titled : **Presentation on Spotify EDA Project**

This Powerpoint will cover some insights I gained from the datasets using SQL, Python, PowerBi and Excel. I will apply the data to try and solve a business questions in relation to TWICE who are a Kpop girls group. In trying to understand what causes songs to rank in the top 10, I will also observe ways that TWICE can increase their streaming numbers, as well as realistic goals that they should set for themselves.

*My objectives*:
1. What are the top 10 songs
2. What factors contribute to streaming number?
3. What recommendations would be useful to TWICE so that their song can reach top 10?

The presentation will cover a range of different visuals which will work together to give insigh on the data and help me build the reccommendations at the end.
The factors looked at in the presentation are: days released, duration, danceability, energy, acousticness and speechiness

## SQL

Titled: **SQL Niyo final Projects - Spotify EDA.sql**

Using BigQuery, I retrieved the dataset and wanted to answer my 3 objectives.

The bigQuery had to be copied to a document as it cannot be dowloaded directly to Github.

Using a range of statements such as SELECT, FROM, LIMIT, GROUP BY, COUNT, ORDER BY, WHERE, BETWEEN, CASE WHEN AND INNER JOIN, I was able to answer the following questions:
1. What are the top 10 most streamed songs?
2. What is TWICE's Current ranking?
3. What factors obviously show an impact on the number of streams? e.g. number of days the song has been released
6. Does the shape of the data have any impact on the ability to visualise it?

The general insights that I recieved from this SQL query was that:
1. The most streamed song was Lucid Dreams by Juice Wrld
2. The highest rank that Twice had gained was 147.
3. Duration had an impact on the total streams: the longer a song has been released, the more streams it is likely to have.
4. CASE WHEN showed that the majority of the Data was within 'less than 100million streams', which suggested that the data set would have to be split to get clearer visuals.

## Excel

Titles **Excel Project Niyo.csv**
Importing the Merged dataframe from python, I used COUNT, MAX and XLOOKUP to note what song had been in the top 10 the most number of times (Heat Waves) which would be useful later in the analysis.

There is a total of 147 different songs within the merged dataframe.

## Python
After importing the necessary dataframes, I merged the dataframes together based on the artist name and song name. After cleaning up the dataframe, I removed rows that I deemed were unecessary. As my project objective was focusing on how to get within the top 10, I thought it unneccessary to have datapoints that are not within top 10, so removed those using loc.

I then used Python to visualise some of the data and derive insights from it.


## PowerBI

To create the dashboard, I imported the original 2 data frames and used them to visualise the correlation between the days and the total streams.
I then imported the merged dataframe from power bi, unpivoted it using Power query and looked at duration and other attributes (Danceability, energy, acousticness, speechiness). I created 2 radar charts and a bar chart to look for trends or similarities.

To create a radar chart specifically looking at TWICE's song, I created a table using Power Query and inputted the data using the origonal dataset from kaggle.

To make the duration chart more readable, I did calculations to convert milliseconds into seconds.

I chose a dark theme to fit with the presentation and the overall theme of the Project.

##Conclusion

This was a challanging project as there was a lot of research that had to be conducted, such as how to make radar and ridgeline plots on powerBI and Python. 

I put a lot of emphasis on making sure my Submissions were readable and aesthetically pleasing to the eye.

I would have liked to look at a dataset with other attributes and comparing them, such as country the artist is form and how long the artist has been in the industry, as i believe there will be strong correlations in that.

I would like to thank Niyo Bootcamps for the support during this project and all the information I learnt during 16 weeks of the bootcamp.
