# AI Trend Analysis Project

## Overview
This project aims to analyze trends in artificial intelligence (AI), machine learning (ML), and related fields by collecting data from multiple sources such as Reddit, Semantic Scholar, and Wikipedia. The goal is to provide insights into public discussions, research developments, and topic popularity over time.

---

## Project Files

### 1. **Reddit Data Collection (`reddit_data.ipynb`)**
- **Purpose**: Collects posts from various AI-related subreddits using the Reddit API.
- **Details**:
  - Monitors subreddits such as *MachineLearning*, *ArtificialIntelligence*, *datascience*, *robotics*, and more.
  - Fetches posts sorted by "new" to ensure the dataset contains the latest discussions.
  - Metadata collected includes:
    - `title`: Title of the Reddit post.
    - `url`: URL of the post.
    - `score`: Net score (upvotes minus downvotes).
    - `num_awards`: Total number of awards received.
    - `created_utc`: Timestamp of post creation.
    - `num_comments`: Number of comments on the post.
    - `subreddit`: Subreddit name.
    - `text`: Body of the post (if available).
- **Output**: A CSV file containing the collected Reddit data.

---

### 2. **Semantic Scholar Data Collection (`semantic_scholar_data.ipynb`)**
- **Purpose**: Retrieves metadata for research papers on AI topics using the Semantic Scholar API.
- **Details**:
  - Queries papers published between 2014 and 2024 across topics like Deep Learning, NLP, Computer Vision, Reinforcement Learning, Generative AI, and more.
  - Metadata collected includes:
    - `title`: Paper title.
    - `authors`: List of authors' names.
    - `year`: Publication year.
    - `citations`: Citation count.
    - `abstract`: Summary of the paper.
    - `venue`: Journal or conference name.
    - `url`: Link to the paper on Semantic Scholar.
- **Output**: A CSV file containing research paper metadata for trend analysis in AI research.

---

### 3. **Wikipedia Data Collection (`wikipedia_data.ipynb`)**
- **Purpose**: Collects Wikipedia pageviews and metadata for AI-related topics using the Wikimedia API.
- **Details**:
  - Starts with seed topics like *Artificial Intelligence*, *Machine Learning*, *Deep Learning*, and expands recursively by following internal Wikipedia links.
  - Metadata collected includes:
    - `article`: Wikipedia page title.
    - `date`: Date of recorded pageviews (YYYYMMDD format).
    - `views`: Number of daily pageviews.
    - `weekday`: Day of the week for each date.
    - Additional metadata: Page ID, creation date, last modified date, URL, description, category, and subcategory.
- **Output**: A CSV file containing daily pageviews and metadata for AI-related topics.
- 
## Outputs
The project generates three main datasets:
1. **Reddit Dataset**: CSV file with posts from monitored subreddits about AI-related discussions.
2. **Semantic Scholar Dataset**: CSV file containing metadata for research papers on various AI topics.
3. **Wikipedia Dataset**: CSV file with daily pageviews and metadata for AI-related Wikipedia pages.
