Twitter Data Analysis Pipeline (Kaggle Dataset)
Project Overview

This project performs data cleaning, transformation, and sentiment analysis on a Kaggle Twitter dataset. The goal is to extract meaningful insights about user engagement and sentiment trends based on tweet content and author activity.

The pipeline processes raw tweet data into structured outputs, including author-level engagement metrics and sentiment scores.

Objectives
Clean and preprocess raw Twitter dataset
Handle missing or irrelevant geographic data
Aggregate engagement metrics (likes, shares) at author level
Perform sentiment analysis on tweet content
Generate structured output datasets for analysis

Dataset
Source: Kaggle Twitter dataset (tweets.csv)
Key fields used:
author
content
likes
shares
latitude, longitude, country (dropped due to missing values)

Project Workflow
1. Data Cleaning
Removed columns with excessive missing values:
latitude
longitude
country
Handled null values in dataset
2. Data Aggregation
Grouped tweets by author
Calculated:
Total likes per author
Total shares per author
3. Sentiment Analysis
Applied sentiment analysis on tweet content
Generated sentiment scores for each author based on their tweets
4. Output Generation

Two processed datasets were created:

Author Engagement Dataset
Author-wise total likes and shares
Sentiment Dataset
Author-wise sentiment scores
Tech Stack
Python
pandas
Natural Language Processing (Sentiment Analysis library used in project)

Outputs

The project generates two CSV files:

author_engagement.csv
Contains aggregated likes and shares per author
author_sentiment.csv
Contains sentiment scores per author

Key Insights (Optional Section You Can Expand Later)
Identified authors with highest engagement
Measured sentiment distribution across users
Explored relationship between engagement and sentiment

How to Run
Install dependencies
pip install pandas

Run main script
python main.py

Project Structure
project/
│
├── tweets.csv
├── main.py
├── data_cleaning.py
├── aggregation.py
├── sentiment_analysis.py
│
├── outputs/
│   ├── author_engagement.csv
│   └── author_sentiment.csv
│
└── README.md
