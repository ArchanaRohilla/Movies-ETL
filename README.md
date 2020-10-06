# Movies-ETL
Automated Extraction, Transformation and Load (ETL) pipeline for movies.
A data pipeline moves data from a source to a destination, and the ETL process creates data pipelines that also transform the data along the way.

## Project Overview
In this project, an automated ETL pipeline has been created that takes in new data, performs the appropriate transformations, and loads the data into existing tables.

## Tools
Python, Pandas, SQL, PostgreSQL

## Summary

### How to run the script:

movies_with_ratings_df = fun_ETL_final('C:/Users/rohil/Desktop/projects/Movies-ETL/wikipedia.movies.json', \
                  'C:/Users/rohil/Desktop/projects/Movies-ETL/movies_metadata.csv','C:/Users/rohil/Desktop/projects/Movies-ETL/ratings.csv')

### The automated ETL pipeline has been created with the following assumptions:

- The wikipedia.movies.json file mostly consists of movies which have 'Director' or 'Directed by' and 'imdb_link' named keys.
- The 'No. of episodes' key in wikipedia.movies.json file does not belongs to movies.
- The values in wikipedia.movies.json have similar information under  different title keys.
- Not every movie got a rating for each rating level.
- Removing the outliers which do not affect the desired data.
- Dropping the duplicate rows based on the 'imdb_link' column.
- Dropping the columns with more than 90% null values.
	  
