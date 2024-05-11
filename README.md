# MOVIE-RECOMMENDATION
# Top Rated Movies Recommendation Project

## Project Overview
The purpose of this project is to recommend top-rated movies based on a dataset containing user ratings and movie titles. The dataset provides information on movie ratings, user IDs, movie IDs, and timestamps. This project focuses on identifying and recommending the highest-rated movies.

## Dataset Information
The dataset for this project consists of two CSV files:
1. `Dataset.csv`: Contains the following columns:
   - `user_id`: A unique identifier for each user.
   - `item_id`: A unique identifier for each movie.
   - `rating`: A rating given by a user to a movie, ranging from 1 to 5.
   - `timestamp`: The timestamp when the rating was recorded.

2. `Movie_Id_Titles.csv`: Contains the following columns:
   - `item_id`: The unique identifier for each movie.
   - `title`: The title of the movie.

## Data Preparation
The following steps were taken to prepare the data for analysis:
- **Data Merging**: Merged the two datasets on the `item_id` column to get the movie titles corresponding to each rating.
- **Additional Columns**: Added columns to the merged dataset to compute the average rating for each movie and the total count of ratings each movie received.
- **Data Deduplication**: Removed duplicate rows to ensure unique records.

## Top Rated Movies
The focus of this project is to identify the top-rated movies. This was achieved by:
- **Sorting Movies by Average Rating**: The dataset was sorted by `average_rating` and `count_rating` in descending order.
- **Selecting Unique Movies**: After sorting, duplicates were removed to ensure that each movie appears only once.

## Recommendation Approach
The primary approach for recommending top-rated movies is to suggest movies with the highest average rating, accounting for the number of ratings received by each movie. This ensures that recommendations are based on a significant number of ratings, reducing the impact of outliers.

## Data Insights
Here are some insights derived from the analysis:
- **Total Movies and Users**: The dataset contains 1,664 unique movies and 944 unique users.
- **Rating Distribution**: Ratings range from 1 to 5, with a significant proportion of ratings being 4 or 5.
- **Top Rated Movies**: A list of the top-rated movies, along with their average ratings and count of ratings.

## Conclusion
This project provides a simple approach to recommending top-rated movies based on user ratings. By focusing on movies with the highest average ratings and considering the count of ratings, recommendations are made based on both popularity and quality.

## Future Enhancements
Possible enhancements to this project include:
- **Movie Recommendations Based on Similarity**: Developing a recommendation system based on movie similarity or user preferences.
- **Exploring Additional Features**: Analyzing additional features like movie genres, directors, or release years to refine the recommendations.
- **User-Centric Recommendations**: Shifting from top-rated movie recommendations to personalized recommendations based on user behavior and preferences.

## Link to the dataset
https://www.kaggle.com/datasets/dev0914sharma/dataset

