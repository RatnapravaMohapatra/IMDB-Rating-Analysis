# IMDB-Rating-Analysis
The IMDB Rating Analysis project focuses on exploring and analyzing movie ratings from the IMDB dataset. The goal is to derive insights into user preferences, trends in movie ratings, and the relationship between movie genres and user-generated tags.
# IMDB Rating Analysis

## Overview
This project analyzes movie ratings from the IMDB dataset to derive insights about user preferences and trends in movie ratings. The analysis utilizes three main datasets: movies, tags, and ratings.

## Datasets
### 1. Movies Dataset
- **Description**: Contains information about movies.
- **Columns**:
  - `movieId`: Unique identifier for each movie.
  - `title`: Title of the movie.
  - `genres`: Genres associated with the movie (e.g., Action, Comedy).
  -  **Example Entry**:
  -  `movieId`: 1, title: Toy Story (1995),genres:Adventure|Animation|Children|Comedy|Fantasy
 
### 2. Tags Dataset
- **Description**: Contains user-generated tags for movies.
- **Columns**:
- `userId`: Unique identifier for each user.
- `movieId`: Unique identifier for the movie being tagged.
- `tag`: The tag assigned by the user.
- **Example Entry**:
- `userId`: 18, movieId: 4141, tag: Mark Waters
  
### 3. Ratings Dataset
- **Description**: Contains ratings given by users to movies.
- **Columns**:
- `userId`: Unique identifier for each user.
- `movieId`: Unique identifier for the movie being rated.
- `rating`: Rating given by the user (scale of 0.5 to 5.0).
- **Example Entry**:
- `userId`: 1, movieId: 2, rating: 3.5
  
## Data Cleaning
- **Removed Unnecessary Columns**: Timestamps were removed from the ratings and tags datasets.
- **Handled Missing Values**:
- Movies and ratings datasets had no null values.
- Tags dataset contained null values, which were dropped to ensure data integrity.

## Descriptive Statistics
- **Ratings Overview**:
- Mean Rating: 3.53
- Rating Range: 0.5 to 5.0
- Most Common Rating: 4.0
- **User  and Movie Statistics**:
- Total Users: 69,045
- Total Movies: 9,041

## Data Visualization
- **Histograms and Boxplots**: Created to visualize the distribution of ratings.
- **Bar Graphs**: Generated to show the frequency of tags used in the dataset.

## Filtering and Aggregation
- **High-Rated Movies**: Filtered movies with ratings greater than or equal to 5.0 for further analysis.
- **Average Ratings**: Grouped ratings by `movieId` to calculate average ratings for each movie.

## Merging Datasets
- **Merged Movies and Tags**: Analyzed the relationship between movie genres and user tags.
- **Merged Average Ratings**: Combined average ratings with movie data to create a comprehensive view of movie performance.

## Insights and Trends
- Identified popular genres based on user ratings and tags.
- Analyzed trends in movie ratings over time to understand shifts in viewer preferences.

## Conclusion
The IMDB Rating Analysis provides valuable insights into user preferences and trends in movie ratings. Future work could involve deeper analysis of specific genres or user demographics to enhance understanding of audience behavior.

## Getting Started
To run this analysis, clone the repository and ensure you have the required libraries installed.


