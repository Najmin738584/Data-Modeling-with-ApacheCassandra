## Data-Modeling-with-ApacheCassandra

A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analysis team is particularly interested in understanding what songs users are listening to. Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app.

This project is aims to create a database schema and ETL pipeline to load song and user data to Cassandra database which make it easy to query and analyze data.


### Datasets

In this project we are working with one dataset: event_data. The directory of CSV files partitioned by date. Here are examples of filepaths to two files in the dataset:

event_data/2018-11-08-events.csv
event_data/2018-11-09-events.csv'

### ETL Process

Extract Step
- Data is extracted from csv file format - event data

Transform Step
- There is no special transformation logic done for this process. The data retrieved from Source files are passed as it is to target tables.

Load Step
- In the Load step, the extracted and transformed data is loaded into the Apache Cassandra tables in sparkify keyspace.


### Environment and Skills
Python, Ipython
Cassandra, cql
