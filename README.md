# SpaceX Launch Data Analysis Project

This project aims to analyze SpaceX's launch data to gain insights into launch success factors and predict launch outcomes. It combines techniques such as web scraping, data wrangling, SQL analysis, data visualization, and machine learning. This repository contains the full project in Jupyter notebooks, each focused on a specific phase of the analysis process.

## Table of Contents
- [Project Overview](#project-overview)
- [File Descriptions](#file-descriptions)
- [Installation and Requirements](#installation-and-requirements)
- [Usage](#usage)
- [References and Acknowledgments](#references-and-acknowledgments)
- [License](#license)

## Project Overview
SpaceX is known for its innovation in aerospace technology, particularly with its Falcon 9 reusable rockets. This project explores SpaceX launch data to identify the variables influencing successful landings and ultimately predict the outcomes of these launches. The analysis and insights generated from this project demonstrate proficiency in data science tools and techniques, from data collection to model building.

## File Descriptions

Each notebook in this repository focuses on a distinct step in the data science workflow:

### 01_Web_Scraping.ipynb
- **Description**: This notebook demonstrates web scraping techniques used to gather data about SpaceX launches. The script fetches data from SpaceX's public APIs and web pages.
- **Key Components**:
  - Imports necessary libraries (`requests`, `BeautifulSoup`, etc.)
  - Scrapes data on launch dates, sites, payloads, outcomes, and other relevant information
  - Saves the scraped data into a CSV file for further analysis

### 02_Data_Wrangling.ipynb
- **Description**: This notebook handles data cleaning and preparation, essential for ensuring data quality before analysis.
- **Key Components**:
  - Reads the data from the CSV file created in the previous step
  - Handles missing values, duplicates, and erroneous data entries
  - Converts data types and formats as needed for analysis
  - Exports a clean dataset for use in exploratory data analysis and modeling

### 03_EDA_SQL.ipynb
- **Description**: This notebook uses SQL queries to explore and analyze the cleaned data.
- **Key Components**:
  - Loads data into a local SQLite database
  - Performs SQL queries to understand the distribution and relationships between variables, such as launch site success rates and payload types
  - Provides summary statistics and insights to inform further analysis steps

### 04_Data_Visualization.ipynb
- **Description**: This notebook creates visualizations to help interpret the data and discover patterns.
- **Key Components**:
  - Visualizes relationships between variables such as payload mass and launch success
  - Uses libraries such as `matplotlib` and `seaborn` for static visualizations
  - Includes charts like bar graphs, scatter plots, and histograms to provide an overview of key insights

### 05_Folium_Visualization.ipynb
- **Description**: This notebook focuses on geospatial data visualization using the Folium library.
- **Key Components**:
  - Maps launch sites and visualizes success rates per location
  - Provides interactive map visualizations, allowing users to explore data geographically
  - Uses markers, pop-ups, and clustering to make the visual experience more informative

### 06_Machine_Learning.ipynb
- **Description**: This notebook builds a machine learning model to predict the outcome of SpaceX launches.
- **Key Components**:
  - Prepares the dataset by splitting it into training and testing sets
  - Trains various machine learning models (e.g., logistic regression, decision tree) to predict launch success
  - Evaluates model performance using accuracy, precision, and recall metrics
  - Exports the trained model and evaluation results for reporting

## Installation and Requirements
To run this project, you will need Python and Jupyter Notebook installed. You can install the necessary libraries by running:

pip install -r requirements.txt

## Key Libraries
- `pandas`, `numpy` for data manipulation
- `requests`, `BeautifulSoup` for web scraping
- `sqlite3` for SQL-based data analysis
- `matplotlib`, `seaborn`, `folium` for data visualization
- `scikit-learn` for machine learning

## Usage
1. **Data Collection**: Run `01_Web_Scraping.ipynb` to gather SpaceX launch data.
2. **Data Cleaning**: Use `02_Data_Wrangling.ipynb` to clean the collected data.
3. **Exploratory Analysis**: Run `03_EDA_SQL.ipynb` to perform SQL-based data analysis.
4. **Visualization**: Use `04_Data_Visualization.ipynb` and `05_Folium_Visualization.ipynb` for static and interactive visualizations.
5. **Machine Learning**: Run `06_Machine_Learning.ipynb` to build and evaluate a model predicting launch success.

## References and Acknowledgments
This project is based on and follows the structure of the IBM Applied Data Science Capstone. I would like to thank IBM Corporation and the original content creators for their valuable guidance and resources.

### Original Project Guiding Authors
- Yan Luo
- Nayef Abou Tayoun
- Joseph Santarcangelo
- Lakshmi Holla
- Pratiksha Verma
- Rav Ahuja

© IBM Corporation 2021-2022. All rights reserved.

## License
This project is licensed under the MIT License - see the LICENSE.md file for details.

