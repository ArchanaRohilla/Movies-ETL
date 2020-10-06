# Movies-ETL
Automated Extraction, Transformation and Load (ETL) pipeline for movies

## Project Overview
In this project, 

## Tools
Python, Pandas, SQL 
## Summary

- How to run the script:

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
	  
