# Data Engineering Nanodegree Project: Data Modeling with Apache Cassandra

This solution comprises a notebook built to practice data modeling in Python over a Cassandra keyspace named `udacity`

## Project Details

### Datasets

For this project, there is only one dataset: `event_data`, which is a directory of CSV files partitioned by date. Here are examples of filepaths to two files in the dataset:

```
event_data/2018-11-08-events.csv
event_data/2018-11-09-events.csv
```

### Project Template

The project template includes one Jupyter Notebook file, in which:

    `event_datafile_new.csv` dataset is processed to create a denormalized dataset
    the data tables are modeled keeping in mind the queries that need to be run
    queries that were needed to model the data tables for are listed
    data is loaded into tables created in Apache Cassandra

## Steps to reproduce

The solution was built using Python 3.8.5 and all dependencies are listed in requirements.txt
To install them, you can run the following command:
```
pip install -r requirements.txt
```

To test it, you can create the database using docker-compose.yaml by running the following command:
```
docker-compose up -d
```

This will create a container named `sparkify-cassandra`.
Next, you will need to run the Jupyter notebook named `Project_1B_ Project_Template.ipynb`. Each step has comments describing all the actions like creating tables over the keyspace and running queries to fetch the results.