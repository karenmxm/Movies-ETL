# Movies-ETL

This project is for the purpose of preparing data for a hackathon. We gathered movies and movie ratings data from both Wikipedia and Kaggle, combine them, and save them into a SQL database.

## Assumptions on unforeseen problems

 1. When calling clean_movies function, users may not use a defined variable names. If happens, ask user to use a defined name.
 2. When extracting imdb_id, there may be a KeyError. 
 3. When parsing dollars, there may be some unforeseen data type error or value error. If happens, assign them NAN.
 4. When filling in missing kaggle_meta data zero values, kaggle_meta data may have other vaule like NAN. If happens, pass this row.
 5. When connecting with PostgreSQL database, handle Exception and psycopg2.Error.
