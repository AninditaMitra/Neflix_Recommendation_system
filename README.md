# Neflix Recommendation System

Over the past few years Netflix has become one of the top online streaming platforms. So it has become important for Netflix to provide recommendations to its users according to their previous watch history. 
Through this project we are trying to understand the usage history of the subscriber along with their current watch. 
We want to learn from the data and recommend the best TV shows to the users, based on self and others behavior.

### Data Description

The dataset consists of four csv files with the following attributes: 
1. Links.csv - 9742 data points (movieId,imdbId,tmdbId)
2. Movies.csv - 9742 data points (movieId,title,genres)
3. Ratings.csv - 100836 data points (userId,movieId,rating,timestamp)
4. Tags.csv - 3683 data points (userId,movieId,tag,timestamp)

### Model Implementation

Alternating Least Squares implementation for Collaborative Filtering is one that fits perfectly in a recommendation engine. 
Due to its very nature, collaborative filtering is a costly procedure since it requires updating its model when new user preferences arrive. 
Therefore, having a distributed computation engine such as Spark to perform model computation is a must in any real-world recommendation engine like the one, we have built here.

### Results

1. Generate top 10 movie recommendations for each user
2. Generate top 10 user recommendations for each movie
