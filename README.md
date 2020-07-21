# Aws Data Warehouse Project

This project created for Udacity Data Engineer course. This project is the third one. 
The document will discuss the following topics:

1. The purpose of this database in the context of the startup, Sparkify, and their decision to move their database to the cloud.  
2. The database schema design and the ETL pipeline.
3. example of queries and results for song play analysis.

___
## Purpose

Sparkify asks for db for better analsys of their users listening habbits. They decided to move their database and ETL pipleine onto AWS. The data will be read from json files in S3, and move into redshift's cluster. Becuase the data come from raw json files, a transformation of the data is needed.

___
## database schema

The database scheme is star-scheme, to improve the queries logic and performance, Which fitting Sparkify request. The star-scheme strogest side is simplicity, which great for queries and aggregations, and because of that better performance. The following diagram show the db structure.  

![DB Scheme](https://i.imgur.com/hBCnPIz.png)

Songplays table is the fact table, while the artists, songs and users are dimension tables.



