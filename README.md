Final LLM Assessment – Employee Sentiment Analysis & Flight Risk Prediction

Project Overview
This project analyzes employee communication data to determine sentiment and engagement levels using Natural Language Processing (NLP) and predictive modeling.
It includes sentiment classification, monthly scoring, employee ranking, flight risk detection, and sentiment trend prediction using regression.

Objectives
Classify messages into Positive, Negative, or Neutral sentiments.
Perform Exploratory Data Analysis (EDA) and data visualizations.
Compute monthly sentiment scores for each employee.
Generate employee rankings based on sentiment levels.
Identify flight risk employees (≥4 negative messages within 30 days).
Build a Linear Regression model for sentiment trend prediction.

Technologies Used
Python
Jupyter Notebook
pandas, numpy – Data preprocessing
vaderSentiment – Sentiment analysis
matplotlib, seaborn – Data visualization
scikit-learn – Regression modeling and evaluation
datetime, os, dotenv – File and environment handling

Methodology

1. Data Preprocessing
Loaded and cleaned the dataset (test.csv).
Extracted employee name, message content, and timestamp.
Converted timestamps to datetime objects and sorted chronologically.

2. Sentiment Labeling
Used VADER Sentiment Analyzer from vaderSentiment library.
Classified each message into Positive, Negative, or Neutral.

3. Exploratory Data Analysis (EDA)
Analyzed message count distribution per employee.
Visualized sentiment distribution and monthly variations using bar and line charts.

4. Monthly Sentiment Scoring
Calculated sentiment scores: Positive = +1, Negative = -1, Neutral = 0.
Aggregated average scores per employee per month.

5. Employee Ranking
Identified Top 3 Positive and Top 3 Negative employees per month.

6. Flight Risk Identification
Flagged employees with ≥4 negative messages within any 30-day period as “At Risk.”

7. Sentiment Trend Prediction
Built a Linear Regression model using scikit-learn.
Predicted sentiment score trends based on message length, frequency, and historical sentiment.

Results
Most employees maintained neutral to positive sentiment.
A few employees exhibited consistent negative sentiment, indicating potential disengagement.
Regression model showed message frequency and length correlate with sentiment scores.

Setup & Usage
1. Prerequisites
Install Python 3.8+ and Jupyter Notebook.
2. Installation
Run the following commands in your terminal:
pip install -r requirements.txt
3. Run the Notebook
Launch the notebook:
jupyter notebook sentiment_analysis.ipynb

Execute all cells to reproduce the analysis, visualizations, and regression model.
