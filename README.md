
# Data Modeling and ETL Project

The goal of this project is to create a database schema and ETL pipeline for a music streaming app called Sparkify. Sparkify wants to analyze the user activity data of the app.



## How to Run
In order to run this pipeline, ```create_tables.py``` and ```etl.py``` need to be run in order.
## Files

### create_tables.py
This script prepares the database by doing the following actions: 
1) Creates the sparkify database. 
2) Establishes connection with the sparkify database and gets cursor to it.  
3) Drops all the tables on the database.  
4) Creates all tables needed and closes the connection.

### etl.py
This script runs the ETL process by doing the following actions: 
1) Extracts data from the json files that contain song data and inserts them to the database.
2) Extracts data from user activity json files. Runs several data transformations on the data and merges it with the song and artist data. Finally, loads the data into the database. 

#### sql_queries.py
This script contains the SQL queries that are utilized by the functions in create_tables.py and etl.py 

