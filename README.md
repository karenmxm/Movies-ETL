# Movies-ETL

This project is for the purpose of preparing data for a hackathon. We gathered movies and movie ratings data from both Wikipedia and Kaggle, combine them, and save them into a SQL database.

## Assumptions on unforeseen problems

 1. New data set may not have any movies.
 2. When changing column name, there may be no current listed columns.
 3. When calling clean_movies function, users may not correctly use variable names. If happens, need user use a defined name.
 4. When parsing dollars, there may be some unforeseen data type error or value error. If happens, assign them NAN.
 5. When filling in missing kaggle_meta data zero values, kaggle_meta data may have other vaule like NAN. If happens, pass this row.
 6. When connecting with PostgreSQL database, handle Exception and psycopg2.Error.
