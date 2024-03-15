# sqlalchemy-challenge
# Project Overview:
This project encompasses climate analysis and the creation of a Flask API to access climate data stored in the Hawaii database.

# Climate Analysis:
The climate analysis segment of the project involves utilizing Python alongside SQLAlchemy to conduct fundamental climate analysis and explore the dataset stored in the climate database. Through the application of SQLAlchemy ORM queries, Pandas, and Matplotlib, various analyses were performed on the dataset.

# Part I: Exploratory Climate Analysis

This phase of the project focuses on analyzing precipitation and weather station data in Hawaii. It involves examining rainfall and temperature patterns to provide insights for planning visits to Hawaii. Key components include:

- SQLite Database (Located at Resources/Hawaii.sqlite)

The database contains relevant climate data for analysis.
- Jupyter Notebook (File: sqlalchemy-challenge/climate_analysis.ipnyb)

Utilizes SQLAlchemy, Python Pandas, and Matplotlib libraries to perform data analysis and visualization.
Analysis Outputs:

-Local precipitation summaries for each weather station.
-Temperature dailies for a customizable range of trip dates.

Visualizations:

Bar charts, histograms, and area charts are generated within the notebook.
Additionally, these visualizations are saved as .png files in the sqlalchemy-challenge folder for easy reference.
![image](https://github.com/Emadkamali/sqlalchemy-challenge/assets/129677932/be754b29-6e9f-47b9-a588-18facc0b668d)

# Part II: Climate App

This phase of the project involves developing a Python Flask application to expose various SQLAlchemy queries related to precipitation and temperature data through an API. The app provides endpoints to access specific climate information, including:

/

Home page.
/api/v1.0/precipitation

Retrieves daily precipitation totals for the last year.
/api/v1.0/stations

Returns a list of active weather stations.
/api/v1.0/tobs

Provides daily temperature observations for the WAIHEE weather station.
/api/v1.0/start

Delivers minimum, average, and maximum temperatures for the range starting from the provided start date.
/api/v1.0/start/end

Presents minimum, average, and maximum temperatures for the range spanning from the provided start date to the end date.
Components include:

SQLite Database (Located at Resources/Hawaii.sqlite)

-Contains the necessary climate data for querying.
- Flask Application (File: sqlalchemy-challenge/app.py)

Implements the endpoints specified above to interact with the database and retrieve relevant climate information.
This climate app facilitates easy access to critical climate data, supporting decision-making processes and enhancing user experience.

