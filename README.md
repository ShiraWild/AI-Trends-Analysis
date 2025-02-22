AI Trends Analysis is a project that collects and analyzes AI-related information from multiple sources, including Wikipedia, research papers, and Reddit discussions. The goal is to track trends in artificial intelligence, identify key topics, and gain insights into the evolution of AI research, public discussions, and technological advancements.

# About the project & repository

Data collection scripts for gathering AI-related content from Wikipedia, research papers, and Reddit.
Preprocessing and cleaning methods to standardize and structure the data.
Exploratory data analysis (EDA) to uncover trends, key discussions, and topic distributions.
Visualization tools to present findings through charts, graphs, and reports.

## Repository Structure
This repository is organized as follows:

- **`data_collection/`**: This directory contains scripts that handle the collection of AI-related data from various sources.
  - **`Reddit_data.ipynb`**: A notebook for collecting data from Reddit.
  - **`semantic_scholar_data.ipynb`**: A notebook for collecting data from Semantic Scholar.
  - **`wikipedia_data.ipynb`**: A notebook for collecting data from Wikipedia.



# 📊 Data Sources & Collection
The data is collected from three primary sources:

## 1️⃣ Wikipedia
Extracts AI-related pages, including machine learning, neural networks, AI ethics, and notable researchers.
Uses web scraping or Wikipedia API to retrieve text and metadata.
## 2️⃣ Research Papers
Collects papers from sources like arXiv, Semantic Scholar, or OpenReview.
Extracts metadata (titles, abstracts, keywords, publication dates).
## 3️⃣ Reddit Discussions
Retrieves AI-related posts from various subreddits using Reddit’s API (asyncpraw).
List of subreddits included in data collection:
MachineLearning, ArtificialIntelligence, DeepLearning, AIethics, datascience, technology, Futurology, and more.
Filters posts by recency and engagement (e.g., upvotes, comments).

# 📑 Metadata Collected

## Wikipedia
Each row represents Wikipedia page page views for a specific date, that was found by following Wikipedia’s internal links from the manually defined source Wikipedia pages (AI-related). 

article: The Wikipedia page title.
date: The date of recorded pageviews in YYYYMMDD format.
views: The number of pageviews for that day.
weekday: The day of the week corresponding to the date.
page_id: A unique identifier for the Wikipedia page.
creation_date: The date when the Wikipedia page was first created.
last_modified: The last time the page was updated.
page_url: The direct link to the Wikipedia page.
description: A short text snippet extracted from the page’s introduction.
category: The first Wikipedia category assigned to the page.
subcategory: The second Wikipedia category (if available)

## Reddit
Each row represents a post in reddit, that belongs to one of the manually defined subreddits (related to AI).

title: post title
url: link to the reddit post 
score: Upvote score - Downvote score (unfourtunately it's not possible to extrat the upvote, downvote scores itself by Reddit API)
num_awards: number of awards received
created_utc: date and time of post creation
num_comments: number of comments on the post
subreddit: name of the subreddit
text: full post content (if available)

## Research Papers
Each row represents a research paper related to manually predefined AI topics.
title
author
years
citations
abstract 
venue
url

# 🚀 Usage & Analysis
1. Data Collection
The scripts collect data in batches over a specified timeframe.
Reddit data is fetched asynchronously using asyncpraw to avoid rate limits.
Wikipedia and research paper data is retrieved via API or scraping.
2. Data Processing
Filters out duplicate or low-relevance entries.
Standardizes timestamps and formats text for analysis.
Extracts topics and trends using NLP techniques (TF-IDF, LDA).
3. Trend Analysis & Visualization
Identifies emerging AI topics over time.
Visualizes popularity trends of key terms.
Generates insights on AI discussions across sources.

# 📌 Installation & Setup

#TODO - fill this
**Requirements**
**Running the Collection Scripts** TODO - explain API credentials

# 📈 Future Improvements
Expand research paper collection to more sources (Google Scholar, IEEE).
Improve topic modeling and trend detection using deep learning.
Automate periodic data collection for continuous tracking.
