# Netflix Database SQL Project
![logo](https://github.com/user-attachments/assets/4e74fe10-572c-4fd9-a32f-59574c9f8174)


This project involves creating and managing a database for Netflix show metadata. The database is designed to store and query information about Netflix shows, including their titles, directors, cast members, release years, and other related metadata. The project uses SQL to create the database, define the schema, and retrieve data.

## Features

- **Database Creation**: The project initializes a database named `netflix_db`.
- **Table Definition**: A table named `netflix` is created with fields to store relevant metadata about Netflix shows.
- **Data Retrieval**: Example queries to interact with and retrieve data from the database.

## Table Schema

The `netflix` table includes the following columns:

- `show_id`: A unique identifier for the show (VARCHAR(5)).
- `type`: The type of content (e.g., Movie, TV Show) (VARCHAR(10)).
- `title`: The title of the show (VARCHAR(250)).
- `director`: The director(s) of the show (VARCHAR(550)).
- `casts`: The cast members of the show (VARCHAR(1050)).
- `country`: The country of origin (VARCHAR(550)).
- `date_added`: The date the show was added to Netflix (VARCHAR(55)).
- `release_year`: The year the show was released (INT).
- `rating`: The rating of the show (VARCHAR(15)).
- `duration`: The duration of the show (VARCHAR(15)).
- `listed_in`: Categories or genres the show belongs to (VARCHAR(250)).
- `description`: A brief description of the show (VARCHAR(550)).

## Usage

1. **Create the Database**:

   ```sql
   CREATE DATABASE netflix_db;
   ```

2. **Create the Table**:

   ```sql
   DROP TABLE IF EXISTS netflix;
   CREATE TABLE netflix (
       show_id VARCHAR(5),
       type VARCHAR(10),
       title VARCHAR(250),
       director VARCHAR(550),
       casts VARCHAR(1050),
       country VARCHAR(550),
       date_added VARCHAR(55),
       release_year INT,
       rating VARCHAR(15),
       duration VARCHAR(15),
       listed_in VARCHAR(250),
       description VARCHAR(550)
   );
   ```

3. **Query the Data**:
   Example:

   ```sql
   SELECT * FROM netflix;
   ```

## Getting Started

To use this project:

1. Install a relational database management system (e.g., MySQL, PostgreSQL).
2. Run the SQL commands provided in the file `sqlQuery_netflix.sql`.
3. Populate the `netflix` table with your data.
4. Execute queries to analyze and explore the data.

## File Structure

- `sqlQuery_netflix.sql`: Contains SQL commands for creating the database and table, as well as sample queries.

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue to improve the project.

##

