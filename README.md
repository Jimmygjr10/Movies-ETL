# Movies-ETL

## Overiview

Amazing Prime loves the dataset and wants to keep it updated on a daily basis. Britta needs your help to create an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables. You’ll need to refactor the code from this module to create one function that takes in the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data—and performs the ETL process by adding the data to a PostgreSQL database.

## ETL_functiion_test
Here we created a function that took in 3 arguments. We then extracted the 3 files we needed to get them in to our pandas dataframe by reading kaggle data and ratings data as CSVs and loading the json file as a DataFrame.
![etl_function](https://user-images.githubusercontent.com/83085800/150984575-59e9c160-c00a-4c04-9810-464009aa9090.png)

## ETL_clean_wiki_movies
In this python file we use list comprehension, functions, and regex to clean movie data and organize column names.
![CleanWikiMovie](https://user-images.githubusercontent.com/83085800/150986163-db0128b3-1fc5-40d2-abfc-a63ec728f3fa.png)

## ETL_create_database
Lastly we used PostgreSQL as our database to load the transformation in. We used sqlalchemy library to create an engine to connect to our database.

![sqlalchemy](https://user-images.githubusercontent.com/83085800/151000663-b7fe42c3-fe73-486a-84c1-687b1b25c83c.png)
