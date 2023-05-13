# nosql-challenge

## Overview

In this project, we have been contracted by the editors of the prestigious food magazine Eat, Safe, Love to evaluate the food hygiene ratings of restaurants across the United Kingdom. Our analysis will assist journalists and food critics in determining their focus for future articles.

The project is divided into three main parts:

## 1. Database and Jupyter Notebook Setup
- Import the provided data "establishments.json" and create a database named "uk_food" with a collection named "establishments".
 - Install the necessary libraries, including PyMongo and Pretty Print.
- Create an instance of the MongoDB Client to establish a connection.
- Confirm the successful creation of the database and collection.

## 2. Update the Database
- Update the database by adding a new halal restaurant called "Penang Flavours" and assign it a business ID and business type.
- Remove any establishments located in the Dover Local Authority.
- Convert the "Longitude," "Latitude," and "Rating Value" fields from string to numeric values.

## 3. Exploratory Analysis
- The "RatingValue" field represents the overall rating decided by the Food Authority, ranging from 1 to 5. Higher values indicate better ratings. Non-numeric values, such as 'Pass,' imply establishments that passed the inspection but didn't receive a numerical rating. We will handle these non-numeric values during the database setup by converting them to null values before converting ratings to integers.

- Conduct the following queries and convert the results into pandas dataframes:

- Identify establishments with a hygiene score equal to 20.
Find establishments in London with a Rating Value greater than or equal to 4.
- Determine the top 5 establishments with a Rating Value of 5, sorted by the lowest hygiene score and proximity to the newly added restaurant, "Penang Flavours."
- Count the number of establishments in each Local Authority area with a hygiene score of 0. Sort the results in descending order and print the top ten Local Authority areas.

## Technologies and Tools
- Programming Language: Python
- Libraries: PyMongo, Pandas, Pretty Print
- Database: MongoDB
- Data Analysis: Exploratory data analysis, Pandas dataframes

By successfully completing this project, we will provide valuable insights to Eat, Safe, Love magazine, assisting them in making informed decisions and enhancing their coverage of UK restaurant food hygiene ratings.