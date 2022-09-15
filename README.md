# Project: Database Modelling with Apache Cassandra
Second project of the Data Engineering Nanodegree from Udacity. 

This project considers an imaginary startup called Sparkify which wants to analyze the data of its music streaming app to understand what songs their users are listening to. Unfortunately the startup has this data only within `csv` files and wants a better way to query it. 

To do so, in this project, an Apache Cassandra NoSQL database is created. This database is called u_de_project_02 and consists of three tables - one for each query to be run:
- Expected result: artist, song title and song's length in the music app history that was heard during  sessionId = 338, and itemInSession  = 4
  - Table name: `songs_by_session`
- Expected result: the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182
  - Table name: `songs_by_user`
- Expected result: user name (first and last) in my music app history who listened to the song 'All Hands Against His Own' 
  - Table name: `users_by_song`

## Files
The project consists of following files:
- `project_02.ipynb` - Notebook with code that creates and manages the Apache Cassandra resources and tables and executes the queries
- `event_data` - Folder that contains `csv` files with the app data
- `envent_datafile_new.csv` - `csv` file generated through the notebook and that contains the relevant data, imported from the files within the `event_data` folder 

## Dependencies
To run the files following libraries (and its dependencies) are necessary:
- `pandas` - Manage dataframes to better display data
- `cassandra-driver` - Connect to Apache Cassandra Database