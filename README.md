# sqlalchemy-challenge
Module 10 Challenge

# Overview of the project 
In this project, we study Honolulu, Hawaii's climate data using Python and SQLAlchemy. We then create a Flask API to show our findings. This project has two maine parts as described below:


# Part 1: Analyze and Explore the Climate Data
In this part, Python and SQLAlchemy is used to do a basic climate analysis and data exploration of a climate database. Specifically, using SQLAlchemy ORM queries, Pandas, and Matplotlib.

1. The provided files (climate_starter.ipynb and hawaii.sqlite) is used to complete climate analysis and data exploration.

2. SQLAlchemy create_engine() function is used as connection to SQLite database.

3. SQLAlchemy automap_base() function is used to reflect tables into classes, and then it saved references to the classes named station and measurement.

4. Python is linked to the database by creating a SQLAlchemy session.

5. Precipitation analysis and then a station analysis are performed by completing the steps in the following two subsections

Precipitation Analysis and Station Analysis

# Part 2: Design Climate App 
After completing the initial analysis, a Flask API based  is designed on the queries that were developed. To do so, use Flask to create your routes as follows:

1. /

Start at the homepage.

List all the available routes.

2. /api/v1.0/precipitation

Convert the query results from your precipitation analysis (i.e. retrieve only the last 12 months of data) to a dictionary using date as the key and prcp as the value.

Return the JSON representation of your dictionary.

3. /api/v1.0/stations

Return a JSON list of stations from the dataset.

4. /api/v1.0/tobs

Query the dates and temperature observations of the most-active station for the previous year of data.

Return a JSON list of temperature observations for the previous year.

5. /api/v1.0/<start> and /api/v1.0/<start>/<end>

Return a JSON list of the minimum temperature, the average temperature, and the maximum temperature for a specified start or start-end range.

For a specified start, calculate TMIN, TAVG, and TMAX for all the dates greater than or equal to the start date.

For a specified start date and end date, calculate TMIN, TAVG, and TMAX for the dates from the start date to the end date, inclusive.

# Files and Folders
The main "SurfsUP" folder includes files and subfolders below:

Folders:
Resources: Contains three data files for analysis and Flask API:
hawaii.sqlite: Climate data in an SQLite database.
hawaii_measurements.csv: CSV file with station, date, precipitation, and temperature data.
hawaii_stations.csv: CSV file listing weather station details, like latitude and elevation.

Files:
app.py: Main file for the Flask API, sets up routes and JSON responses.
climate_starter.ipynb: Jupyter Notebook with Python code for climate analysis.

# Tools 
Programming Language: Python
Libraries: Pandas, NumPy, Matplotlib, SQLAlchemy, Flask
Database: SQLite
Development Environment: Jupyter Notebook, Visual Studio Code