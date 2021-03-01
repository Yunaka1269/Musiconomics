# Final_Project: Musiconomics

## Topic 
The topic we have selected for the final project is looking into how music data has evolved over the past 100 years. The purpose of this analysis is to understand and examine different attributes of music, including genres, energy, loudness, tempo, and danceability, to name a few. 

## Reason
We decided on this topic due to all team members' mutual interest in music and curiousity on musical trends over the decades. Further, we also identified that the data that was accessible to us included many variables and factors to perform deeper analysis on. 


## Data Sources
- Data from data_by_artist.csv, data_by_genres.csv, data_by_year.csv and data_w_genres.csv 


## Questions
- What are the correlations between popularity and audio features?
- Does the duration of songs change over the years?
- What artist are most popular?

# Technologies Used


## Machine Learning Model 
- Yu


## Database

![Spotify Artist and Song ERD](https://github.com/zanelouis/Final_Project/blob/Keshs_branch/Spotify_Data_ERD.png)

The snapshot above represents the entity relationship diagram (ERD) for the Spotify data analysis project, and includes three tables for - 
#### Artist Data
One artist can have many songs and many genres

#### Song Data
One song can have many artists and many genres

#### Genre Data
One genre can have many artists and many songs

We will be housing the data in a SQL database (Postgres) and we hope to integrate it with Tableau to display and visualize the data

## Data Cleaning and Analysis
Pandas will be used to clean the data and perform an exploratory analysis. Further analysis will be completed using Python.


## Machine Learning
SciKitLearn is the ML library we'll be using to create a classifier. 


## Dashboard
We intend to use Tableau as our dashboard to present the data visualizations created throughout the course of this project.  
