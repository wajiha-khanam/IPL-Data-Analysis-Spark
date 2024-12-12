# IPL Data Analysis with PySpark

This project performs exploratory and analytical tasks on IPL (Indian Premier League) cricket data using PySpark. It leverages Spark's powerful distributed processing capabilities to analyze large datasets and visualize the insights.

---

## Project Overview

The objective of this project is to analyze IPL match data, player statistics, and team performances to extract meaningful insights. It covers:

- Preprocessing and transforming datasets.
- Statistical analysis such as identifying top-performing players, understanding toss impacts, and scoring trends by venue.
- Visualization of results using Python libraries  ( Matplotlib and Seaborn ).

---

## Data Sources

The project uses the following datasets (stored in AWS S3 buckets):
- **Ball by Ball Data:** Details of each ball bowled during matches.
- **Match Data:** Summarized match information, including teams, dates, and results.
- **Player Data:** Information about players, including batting and bowling styles.
- **Player Match Data:** Player statistics for individual matches.
- **Team Data:** Team names and details.

---

## Features and Analysis

### 1. Data Preprocessing
- Loaded datasets using `spark.read` with appropriate schemas.
- Filtered and normalized data (e.g. excluding wide/no-balls for specific analysis).
- Handled missing values and added derived columns (e.g. categorizing batting hand, age-based veteran status).

### 2. Analytical Insights
- **Top Scorers Per Season:** Identified the highest-scoring batsmen for each season.
- **Economical Bowlers in Powerplay:** Analyzed bowlers' performance in the first 6 overs.
- **Impact of Toss:** Explored the correlation between winning the toss and winning the match.
- **Runs in Winning Matches:** Evaluated players with the highest average runs in wins.

### 3. Venue Analysis
- Computed average and highest scores by venue to highlight scoring trends.

### 4. Dismissal Analysis
- Analyzed the most frequent types of dismissals across matches.

### 5. Team Toss Performance
- Assessed team performance after winning the toss.

---

## Visualization

The project uses `Matplotlib` and `Seaborn` for visualization. Key plots include:
- Bar charts for top performers (batsmen, bowlers).
- Count plots showing toss impacts.
- Venue-wise score distributions.
- Dismissal frequency distributions.

---

## Running the Project

### Prerequisites
- **Environment:** Databricks Notebook.
- **Python Libraries:** Pandas, Matplotlib, Seaborn.
- **Data Storage:** Access to IPL data stored in an S3 bucket.

---


## Author

- **[Wajiha Khanam]**

---
