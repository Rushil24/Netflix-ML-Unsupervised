# Netflix Content Analysis & Prediction using Machine Learning & GenAI
## Project Overview

This project analyzes Netflix’s Movies and TV Shows dataset to uncover patterns, trends, and insights that can help in content recommendation, production strategy, and user engagement. Using Machine Learning (ML) models and Generative AI techniques, the project classifies content, analyzes duration, release years, genre trends, and predicts content types.

## Problem Statement

Netflix has an ever-growing library of Movies and TV Shows. Understanding production trends, genre popularity, and content characteristics is crucial for decision-making, content recommendation, and improving user experience. The goal is to analyze Netflix content data, extract actionable insights, and build ML models to classify content effectively.

## Dataset Description
The dataset contains the following features:

Column	Description
show_id	Unique ID for each Movie/TV Show
type	Movie or TV Show
title	Name of the Movie/Show
director	Director of the show
cast	List of actors
country	Country of production
date_added	Date it was added on Netflix
release_year	Actual release year
rating	TV rating of the show
duration	Minutes or Seasons
listed_in	Genre(s)
description	Summary description
Project Steps

## Data Wrangling & Preprocessing

Handle missing values (e.g., director → unknown, cast → not listed).

Standardize date and duration formats.

Outlier detection and treatment for duration and release_year.

Categorical encoding for country, rating, and director.

Text preprocessing for description and listed_in including lowercasing, punctuation removal, stopword removal, tokenization, normalization, and vectorization.

## Feature Engineering

Extract year/month from date_added.

Create binary column is_movie (Movie=1, TV Show=0).

Count number of actors.

Extract primary genre from listed_in.

## Exploratory Data Analysis (EDA)

14+ visualizations including distribution plots, countplots, pairplots, correlation heatmap, outlier analysis.

Insights on top genres, countries, duration trends, number of actors, and yearly content growth.

## Hypothesis Testing

Tested differences in duration, number of actors, and release year between Movies and TV Shows using t-tests.

## Machine Learning Models

Random Forest, SVM, Logistic Regression for content type prediction.

Hyperparameter optimization using RandomizedSearchCV for SVM and GridSearch for others.

Evaluation using Accuracy, Precision, Recall, F1 Score, with visual metric comparison charts.

## Key Insights

Movies and TV Shows differ significantly in duration and release years.

The number of actors does not significantly vary between Movies and TV Shows.

Top genres and production countries help guide content acquisition and production strategies.

ML models achieved high accuracy (~97-98%), validating their use for content classification and recommendation.

## Business Impact

Helps Netflix in content strategy, ensuring popular genres and production countries are prioritized.

Improves recommendation engines using ML predictions.

Reduces manual effort for classifying new content.

Provides insights for marketing campaigns based on release trends and user preferences.

## Technologies Used

Python – Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, NLTK

Machine Learning – Random Forest, SVM, Logistic Regression, Hyperparameter Tuning

Generative AI – Text preprocessing & vectorization for NLP tasks

Visualization – Distribution plots, Countplots, Pairplots, Heatmaps

## Run Jupyter Notebook Netflix_Capstone_Project.ipynb to see the analysis, ML model training, and evaluation.

### Author

Rushil Pajni
