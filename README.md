# Final_Project: Musiconomics

Please visit this [link to the tableau dashboard](https://public.tableau.com/views/Group_16156329936470/Audio_Features_Year?:language=en&:display_count=y&:origin=viz_share_link "link to tableau dashboard" )
and [link to the Google Slides](https://docs.google.com/presentation/d/1p_Z2Gktkt6Z4mRQBZBdKG34dpdG-liZxhFf-hvlsZvU/edit?usp=sharing?publish=yes "link to Google Slides") for presentation content.

## Topic 
The topic we have selected for the final project is looking into how music data has evolved over the past 100 years. The purpose of this analysis is to understand and examine different attributes of music, including genres, energy, loudness, tempo, and danceability, to name a few. 

## Reason
We decided on this topic due to all team members' mutual interest in music and curiosity on musical trends over the decades. Further, we also identified that the data that was accessible to us included many variables and factors to perform deeper analysis on. 


## Data Sources
Data from Kaggle [linked here](https://www.kaggle.com/ironicninja/icm-problem-d "linked here") titled "The Influence of Music, Spotify and AllMusic Data" includes files:
- music_genre.csv
- influence_df.csv
- prediction.csv
- data_by_artist.csv
- data_by_year.csv 


## Questions
- What are the correlations between genre and audio features from the past 100 years?
- What music eras are considered?
- What variables are found in the Spotify data?
- What insights are drawn from correlation analysis?

# Technologies Used


## Machine Learning Model 
- Apply linear regression model on the eight distinct audio features (danceability, energy, valence, loudness, acousticness, instrumentalness, liveness, speechiness).


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

After the initial design analysis was performed on the data, and once the ERD was set up, the approach was altered based on the availability of a more viable option -

The approach taken for setting up the database is as follows - 
1) Analyzed different databases available - Postgres and SQLite were the two databases that were considered and after analyzing the data size and flexibility, I decided to proceed with the SQLite approach as it offered more flexibility and the size of the data isn't too large to necessitate Postgres
2) Two separate tables containing music genre data and influencer data were created and the csv data loaded into the tables through Pandas DataFrames
3) Values were fetched from the SQLite tables using the fetchall() function
4) Join was created between the two tables and will need to be analyzed further to see the impact of the join and if the type of join needs to be modified to get the most out of combining the two datasets

### Further Analysis Needed
Joins - In the coming week, further analysis needs to be performed to understand the impact of the join created and see if the type of join or the data that is being joined with the music_genre data needs to be revised


## Machine Learning
Compare accuracy rate on following Scikit-learn Machine Learning models and determine which one returns the best performance. The analysis is based on songs (data) released after year 2000 onwards.
- RandomForest Classifier
- Gradient Boost
- SVM
- Logistic Regression
- DecisionTree Classifier


## Dashboard
We intend to use Tableau as our dashboard, with additional visualizations from Python libraries, to present the data visualizations created throughout the course of this project.  The storyboard of the dashboard is included in the Google Slides presentation linked above. 
- Tools Used: Tableau, Python Matplotlib, Seaborn, Scikit-learn Libraries
- Interactive Elements: Filtering by year to display the audio feature distribution over time

