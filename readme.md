# ELT (Extract, Load, and Transform) Pipeline 

This project demonstrates an **End-to-End ELT pipeline** for a Netflix Movies and TV Shows dataset. The process involves extracting the data, loading it into a raw layer, transforming the data through cleaning and modeling, and finally analyzing the data using SQL.

## Project Overview

### Data Source:
- **Dataset**: [Netflix Movies and TV Shows dataset](https://www.kaggle.com/datasets/shivamb/netflix-shows), which contains a regularly updated list of movies and shows available on Netflix.

- **Objective**: To perform ETL (Extract, Transform, Load) and analyze the dataset through SQL queries.

### Process Workflow:

1. **Extract (Download Dataset)**:
   - The dataset is downloaded from an external source using **Python**.
   
2. **Load to Raw Layer**:
   - The downloaded dataset is loaded into the **Raw Data Layer** in an **SQL Server** using **Python**.

3. **Data Cleaning, Modelling, and Transformations**:
   - Data is cleaned, transformed, and stored in the **Final Staging Layer** of the SQL Server for further analysis.
   - The transformation process involves a series of steps for data preparation.

4. **Data Analysis using SQL**:
   - After cleaning and transformation, data analysis is carried out using SQL queries.
   - We answer **5 specific SQL questions** to derive insights from the dataset.

## Data Cleaning and Transformations

The following transformations and cleaning tasks were applied to the dataset to prepare it for analysis:

1. **Handling Foreign Characters**:
   - Special or non-ASCII characters in the dataset are identified and handled appropriately to avoid encoding issues.

2. **Removing Duplicates**:
   - Duplicate entries in the dataset are removed to ensure that each record is unique and accurate.

3. **Data Type Conversion**:
   - Converting the data into the correct formats (e.g., dates, integers, strings) for better analysis.
   
4. **Identifying and Populating Missing Values**:
   - Missing values in the dataset are either filled with suitable values or handled to avoid errors during analysis.

5. **New Dimension Table for Countries**:
   - A new dimension table is created for countries, allowing for country-based filtering and more meaningful analysis.

## Data Analysis using SQL

After performing the necessary data transformations, the following **5 SQL questions** were answered using the cleaned dataset:

1. **What is the total number of movies and TV shows available on Netflix?**
   - A count of all records in the dataset, distinguishing between movies and TV shows.

2. **Which country has produced the most content on Netflix?**
   - A query to find out which country has the highest number of Netflix titles.

3. **What is the most common genre on Netflix?**
   - Identifying the genre that appears most frequently across all movies and TV shows.

4. **How many movies were released in the year 2020?**
   - A query to count the number of movies added to Netflix in 2020.

5. **What is the distribution of movie durations?**
   - Analyzing the range and distribution of durations for movies to gain insight into common length patterns.

