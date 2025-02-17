# WIDS 2024 Netflix Content Strategy Analysis with Python 
Our Content Strategy Analysis project aims to investigate how streaming platforms, particularly Netflix, create, release, distribute, and consume content to achieve their strategic goals. We'll analyze various elements of Netflix's content strategy, focusing on maximizing audience engagement, viewership, brand reach, and revenue. This analysis provides valuable insights for anyone interested in the media and entertainment industry or looking to enhance their understanding of content strategy through Python.

Join us as we explore these fascinating topics, and feel free to contribute or ask questions!

# Resources
# Week 1 Python and Key Libraries for Data Analysis
Aim: Build a foundation in Python programming and essential libraries for data analysis and visualization.

### Important Links
* [Python Tutorial for Beginners](https://youtu.be/vLqTf2b6GZw?feature=shared) <br/>
* [Pandas Tutorial](https://www.youtube.com/watch?v=vmEHCJofslg&t=767s) <br/>
* [Numpy Tutorial](https://youtu.be/QUT1VHiLmmI) <br/>
* [Matplotlib Tutorial](https://youtu.be/3Xc3CA655Y4?feature=shared) <br/>

### Week 1 Assignment
## Task Overview
You are provided with a dataset. Your goal is to perform the following analyses using Python: 
1. Highest Elo

Identify the player with the highest Elo rating in the dataset.

2. Top 10 Players With Highest Elo

List the top 10 players with the highest Elo ratings.

3. Time Trend of Top 10's Average Elo Each Year

Plot how the average Elo of the top 10 players has changed over the years.

4. Time Trend for Number of Players Above 2750 Elo

Visualize the trend for the number of players exceeding 2750 Elo each year.

5. Time Trend of Top 10's Average Age Each Year

Analyze the change in the average age of the top 10 players year by year.

6. Time Trend for Number of Players Under 25 Years Old in Top 10

Observe how the number of top 10 players under 25 years of age has changed over the years.

7. Time Trend of Magnus Carlsen's Elo

Track Magnus Carlsen's Elo rating over time.

## Note
* The Date column contains values stored as strings in the format YYYY MMM (e.g., 2020 Jan). To analyze time trends:
1. Extract the year by slicing the first four characters from the date string (e.g., 2020 from 2020 Jan).
2. Convert the resulting year values into integers.

## Deliverables
* Submit a Python notebook or equivalent code with your solutions.
* Include visualizations for all time trend questions.
* Provide a brief interpretation of the trends observed in each plot.

# Week 2
# Objective 
In this assignment, you will practice cleaning and preprocessing data using the Global Land Temperatures by Country dataset. The focus will be on handling inconsistencies, parsing date information, and preparing the dataset for analysis.

## Tasks
1. Load the Dataset
* Import the dataset using Pandas.
* Display the first 10 rows and use .info()/.describe() method to examine statistical information and the structure of the dataset.

2. Handle Missing Values
* Identify columns with missing values. <br/>
  [Handling missing values in dataset](https://youtu.be/uDr67HBIPz8?feature=shared) <br/>
  Analyze the missing data pattern and using a method that you find logical or beneficial for further analysis. <br/>

3. Parse the Date Column
* Convert the "dt" column (datetime string) into a proper datetime format.
  [Tutorial](https://youtu.be/fNzUhp5uHFY?feature=shared) <br/> 
* Extract and create new columns for: <br/>
  Year <br/>
  Month <br/>
  Day (if necessary) <br/>
  Example: Split 1750-01-01 into Year = 1750, Month = 1. <br/>

4. Check for Data Consistency
* Filter Data Based on Uncertainty <br/>
  Define a threshold for acceptable uncertainty (e.g., AverageTemperatureUncertainty ≤ 2.0). <br/>
  Filter out data points with uncertainty above this threshold. <br/>
  Report the size of the dataset before and after filtering. <br/>
  Justify the chosen threshold and discuss its impact on data quality. <br/>
  * Hints <br/>
    Identify rows with AverageTemperatureUncertainty > 2.0. <br/>
    Create a new filtered DataFrame excluding these rows. <br/>
    Print the size of the original dataset vs. the filtered dataset. <br/>

* Visualize Temperature Trend with Uncertainty <br/>
  * Group the dataset by Year and calculate: <br/>
   Mean of AverageTemperature. <br/>
   Mean of AverageTemperatureUncertainty. <br/>
   Plot the average temperature trend over time with error bars representing uncertainty. <br/>
   * Hints <br/>
     Use Matplotlib’s errorbar function to plot the temperature trend with uncertainty. <br/>
     Highlight years where uncertainty is exceptionally high. <br/>

* Analyze Trends in Uncertainty <br/>
  Plot the trend of AverageTemperatureUncertainty over time separately. <br/>
  Observe whether uncertainty has increased or decreased over time and hypothesize why (e.g., improved measurement techniques). <br/>
  * Hints: <br/>
    Group data by Year and calculate the mean uncertainty. <br/>
    Plot the yearly uncertainty trend. <br/>

* Identify High-Uncertainty and Inconsistent Periods <br/>
  * Identify years where: <br/>
    The mean uncertainty exceeds a reasonable threshold. <br/>
    Temperature values show significant fluctuations (e.g., large outliers). <br/>
  * Discuss the potential reasons for these inconsistencies and their relationship with uncertainty. <br/>
    
5. Export the Cleaned Data <br/>
   * Save the cleaned dataset to a new file (e.g., cleaned_temperatures.csv). <br/>
   * A Python notebook or script containing: <br/>
    Data filtering based on uncertainty. <br/>
    Trend analysis of average temperature with error bars. <br/>
    Analysis of uncertainty trends over time. <br/>
    Identification of high-uncertainty and inconsistent periods. <br/>
  * A line graph of average temperature with error bars representing uncertainty. <br/>
  * A separate line graph showing the trend in uncertainty over time. <br/>
  * Insights and explanations on how uncertainty impacts data consistency and analysis. <br/>
