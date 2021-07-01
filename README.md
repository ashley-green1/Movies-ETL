# Movies-ETL

## Overview

I have been tasked with creating an automated ETL pipeline that creates a Movie database from both structured and unstructured data. 
Code is written that extracts Wikipedia JSON data, Kaggle metadata, and the MovieLens rating data, transforms the data with regex and functions, then lastly, loads the data into a PostgreSQL database.

## Resources

- Extract - ETL_function_test.ipynb <br>
- Transform - ETL_clean_wiki_movies.ipynb & ETL_clean_kaggle_data.ipynb <br>
- Load - ETL_create_database.ipynb <br>

- Languages: Python, SQL
- Tools: Jupyter Notebook, JSON, Pandas, NumPy, sqlalchemy, psycopg2
- Data Source(s): wikipedia.movies.json, movies_metadata.csv, ratings.csv (note: due to large file size, I am unable to push ratings.csv to repo)


## Results

The resulting database consists of two tables that are highlighted below.

A movies table with 6,052 rows of data, each representing a unique movie title. The table also includes 31 columns of data with production related information, such as, movie budget, producers, actors and release data. 

![movies](https://github.com/ashley-green1/Movies-ETL/blob/main/Resources/movies_query.png)

A ratings table a table with 26,024,289 rows of data, each representing a viewer rating of 1-5. The table also includes 5 columns of data such as movie title, rating and date.
![ratings](https://github.com/ashley-green1/Movies-ETL/blob/main/Resources/ratings_query.png)
