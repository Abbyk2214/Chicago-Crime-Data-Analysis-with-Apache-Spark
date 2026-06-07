# Chicago Crime Data Analysis with Apache Spark

## Project Overview

This project analyzes Chicago crime data using Apache Spark. The goal was to practice working with large-scale data by loading, cleaning, transforming, and analyzing more than one million crime records from the City of Chicago crime dataset.

The analysis focuses on crime trends over the last ten years, the time of day when crimes occur most often, and the most common crime types in the dataset.

## Dataset

The dataset used in this project comes from the City of Chicago Data Portal:

Chicago Crimes - 2001 to Present  
https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-Present/ijzp-q8t2/data

The dataset includes crime records reported in Chicago, including information such as date, location, primary crime type, arrest status, and year.

## Tools Used

- Python
- Apache Spark / PySpark
- Google Colab
- Matplotlib
- Pandas

## Project Steps

## 1. Created a Spark Session

A Spark session was created to process the dataset using PySpark.

## 2. Loaded the Dataset

The Chicago crime dataset was loaded into a Spark DataFrame. The dataset contained more than one million records.

## 3. Cleaned the Data

The data cleaning process included:

- Removing null values
- Converting the `Date` column to a timestamp data type
- Filtering the dataset to include only the last ten years
- Removing selected crime types:
  - NON-CRIMINAL (SUBJECT SPECIFIED)
  - OTHER OFFENSE
  - STALKING
  - NON - CRIMINAL
  - ARSON
- Merging similar crime types, such as combining `SEX OFFENSE` and `PROSTITUTION` into one category

## 4. Analyzed Crime Trends

The cleaned dataset was used to answer the following questions:

- How has crime changed year by year over the last ten years?
- What hour of the day has the highest number of crimes?
- What are the top ten most common crime types?

## Results

The analysis showed year-wise crime trends, identified the hour with the highest crime activity, and displayed the top ten most common crimes in a bar chart.

## Visualizations

A bar chart was created to show the top ten crime types in the dataset.

## Key Skills Demonstrated

- Big data processing with Apache Spark
- Data cleaning and transformation
- Working with timestamps and date filtering
- Grouping and aggregating large datasets
- Data visualization with Matplotlib
- Using Google Colab for Spark analysis

## How to Run This Project

1. Open the notebook in Google Colab.
2. Install and set up PySpark.
3. Load the Chicago crime dataset from the City of Chicago Data Portal.
4. Run each notebook cell in order.
5. View the final analysis and visualizations.

## Conclusion

This project helped demonstrate how Apache Spark can be used to process and analyze large datasets efficiently. By using PySpark, I was able to clean the Chicago crime dataset and identify meaningful crime patterns based on year, hour, and crime type.
