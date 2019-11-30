# WeekendMovieTrip
Clustering models based on movie ratings 

# Weekend Movie Trip
  
1. Set up a data science project structure in a new git repository in your GitHub account
2. Download the one of the MovieLens datasets from https://grouplens.org/datasets/movielens/
3. Load the data set into panda data frames
4. Formulate one or two ideas on how the combination of ratings and tags by users helps the data set to establish additional value using exploratory data analysis
5. Build one or more clustering models to determine similar movies to recommend using the other ratings and tags of movies by other users as features
6. Document your process and results
7. Commit your notebook, source code, visualizations and other supporting files to the git repository in GitHub

# Feature Engineering 
  The steps I took toward feature engineering in this project were:
  1. I removed timestamps from my datasets as they interfered with the merging of my data sets. Ratings and tags on movies are not reliant on the time at which the movie was watched or rated.
  2. Merged my data sets together based on MovieId. Since the assignment was to create movie recommendations, the most important attribute in these sets was the movies themselves.
  3. Label encoded the Tags and titles so I could feed them into my model.
  
 # Clustering Models
    I chose to build my clusters based on ratings and tags of movies. It reasons that a person who rates a movie with certain tags very highly, they will enjoy watching movies with similar tags that have also been ranked highly by other viewers. If someone would like to use my model, they must find the cluster containing a movie they like, then choose another movie located in the same cluster. 
