# Game Analytics: Unlocking Tennis Data with SportRadar API 🎾

## Problem Statement:
# The SportRadar Event Explorer project aims to develop a comprehensive solution for managing, analyzing sports competition data extracted from the Sportradar API.The application will parse JSON data, store structured information in a relational database, and provide intuitive insights into tournaments, competition hierarchies, and event details.This project is designed to assist sports enthusiasts, analysts, and organizations in understanding competition structures and trends while exploring detailed event-specific information interactively.

## Skills Takeaway:
# 1. Data Extraction: Extracting data via API calls / Making API requests to collect data.
# 2. SQL Database Management: Create tables and a schema to organize data in a structured format.
# 3. Data Analysis: Writing SQL queries to derive insights.
# 4. Application : Build a Streamlit Application.


## Technical Tags:
# API Integration: Sportradar API-Key
# Languages : Python(Pandas,tabulate,mysql.connector)
# Database: MySQL/PostgreSQL
# Application: Streamlit

## Approach (My Work):

## Data Extraction:
# Sign up and log in Sportradar Website to access a free API key valid for 30 days.
# Request data from Sportradar's API using the provided API key.The API provides the fetched data in JSON format.
# Transform nested JSON structures into a table format for further analysis.

## Data Storage: 
# Use 'mysql.connector' library in Python to connect to the MySQL server and perform database operations within the Python environment.
# Design a SQL database with relational tables, ensuring the use of correct data types, primary keys, and foreign key constraints.
# Tables:
     # 1. Categories Table [['category_id','category_name']]
     # 2. Competitions Table [['competition_id','competition_name','parent_id','type','gender','category_id']]
     # 3. Complexes Table [['complex_id','complex_name']]
     # 4. Venues Table [['venue_id','venue_name','city_name','country_name','country_code','timezone','complex_id']]
     # 5. Competitor_Rankings Table [['rank_id','rank','movement','points','competitions_played','competitor_id']]
     # 6. Competitors Table [['competitor_id','name','country','country_code','abbreviation']]
# Primary Key: A Primary Key is a column (or a combination of columns) in a table that uniquely identifies each record. It must contain unique values and cannot have NULL values. The primary key ensures that each row in the table is distinct.
# Foreign Key: A Foreign Key is a column (or a combination of columns) in a table that establishes a link between data in two tables. It references the Primary Key of another table, creating a relationship between them.The foreign key acts as a "bridge" between two tables, allowing them to be connected logically. It ensures that data in the related tables remains consistent and that relationships between the tables are maintained.

## Data Analysis:
# Write SQL queries to derive meaningful insights.
# Use SQL JOIN operations on related tables, where the primary key in one table links to the foreign key in another, to derive insights
# Use the Python 'tabulate' package to display the retrieved data in a structured table format in Python environment.

# Build a Streamlit Application :
# Connect the Streamlit app with the SQL database for real-time query execution.
# Display analysis results in the form of tables, charts, or dashboards within the app.User Interface: Interactive dashboards with filters for competition types, levels, and categories.
# Features for the Application:
  # Search and Filter Competitors :Allow users to search for competitors by name or display a list of all features.
  # Ensure a smooth navigation experience with interactive features for effective data display and analysis.


## Results :
 #The expected outcome is a fully functional web application capable of parsing and visualizing sports event data. Users can navigate competition hierarchies, filter data, and generate meaningful insights about sports events. This project will enhance proficiency in working with APIs, databases, and visualization tools.

       
