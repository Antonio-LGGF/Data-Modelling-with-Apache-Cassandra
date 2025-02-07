# Project: Data Modeling with Apache Cassandra

# Datasets
For this project, you'll be working with one dataset: **"event_data"**. This dataset consists of CSV files partitioned by date. Here are examples of file paths for two files in the dataset:

- `event_data/2018-11-08-events.csv`
- `event_data/2018-11-09-events.csv`

# Project Template
To get started with the project, go to the workspace on the next page, where you'll find the project template (a Jupyter Notebook file). You can work on your project and submit your work through this workspace.

The project template includes one Jupyter Notebook file, in which:

- You will process the **"event_datafile_new.csv"** dataset to create a denormalized dataset.
- You will model the data tables, keeping in mind the queries you need to run.
- You have been provided queries that you will need to model your data tables for.
- You will load the data into tables created in **Apache Cassandra** and run your queries.

# Project Steps
Below are the steps you can follow to complete each component of this project.

## Modeling Your NoSQL Database (Apache Cassandra)
1. Design tables to answer the queries outlined in the project template.
2. Write Apache Cassandra **CREATE KEYSPACE** and **SET KEYSPACE** statements.
3. Develop **CREATE** statements for each table to address each question.
4. Load the data using **INSERT** statements for each table.
5. Include **IF NOT EXISTS** clauses in your **CREATE** statements to create tables only if they do not already exist. We recommend also including a **DROP TABLE** statement for each table so that you can drop and recreate tables whenever needed to reset your database and test your ETL pipeline.
6. Test by running the appropriate **SELECT** statements with the correct **WHERE** clauses.

## Build ETL Pipeline
1. Implement the logic in **Part I** of the notebook template to iterate through each event file in **"event_data"**, process it, and create a new CSV file in Python.
2. Make necessary edits to **Part II** of the notebook template to include Apache Cassandra **CREATE** and **INSERT** statements to load processed records into relevant tables in your data model.
3. Test by running **SELECT** statements after executing the queries on your database.
