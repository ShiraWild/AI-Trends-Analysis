### **AI Trends Analysis**

1. **`data_analysis/`**
   - Contains the analysis script `AITrendsAnalysis_analysis.ipynb`.
   - This script processes the collected datasets to extract insights, visualize trends, and perform comparative analyses across sources.

2. **`data_collection/`**
   - Contains scripts for collecting data:
     - `reddit_data.ipynb`: Fetches posts from AI-related subreddits using the Reddit API.
     - `semantic_scholar_data.ipynb`: Retrieves metadata for research papers on AI topics using the Semantic Scholar API.
     - `wikipedia_data.ipynb`: Collects daily pageviews and metadata for AI-related topics via the Wikimedia API.

3. **`visualizations/`**
   - Contains visualizations generated during analysis.
   - Includes plots in both HTML and PNG formats for easier sharing and embedding.

---
## Collected Data - Reddit, Wikipedia and Scholar

The data is too large to upload it to git repository. To explore the data itself, you can find it in this drive directory with read access through this link:
https://drive.google.com/drive/folders/1RuXT5ZJHMu8nvCY58EcIzrAs_mulu3Co?usp=drive_link

## File Descriptions

### **Data Collection Scripts**

1. **`reddit_data.ipynb`**
   - Collects posts from AI-related subreddits such as *MachineLearning*, *ArtificialIntelligence*, *datascience*, etc.
   - Captures metadata including post title, URL, score, number of comments, awards, and subreddit name.

2. **`semantic_scholar_data.ipynb`**
   - Fetches research papers published between 2014–2024 on topics like Machine Learning, NLP, Computer Vision, etc.
   - Metadata includes title, authors, year of publication, citation count, abstract, venue, and URL.

3. **`wikipedia_data.ipynb`**
   - Collects pageviews and metadata for AI-related Wikipedia topics.
   - Captures daily pageviews over the past decade along with metadata such as article title, creation date, last modified date, categories, and description.

### **Data Analysis Script**

4. **`AITrendsAnalysis_analysis.ipynb`**
   - Analyzes the collected datasets to uncover trends in public interest (Reddit), research activity (Semantic Scholar), and topic popularity (Wikipedia).
   - Performs tasks such as:
     - Visualizing trends over time.
     - Comparing engagement levels across platforms.
     - Identifying emerging topics in AI.

---

## Applications

- **AI Domains Public Interest Analysis**: Understand which AI topics are gaining traction on social media platforms like Reddit.
- **Research Trends**: Identify emerging areas in AI research based on publication activity and citation counts from Semantic Scholar.
- **Topic Popularity Tracking**: Use Wikipedia data to study how interest in specific AI concepts evolves over time.
and more ...
---

## Outputs

The project generates three main datasets:
1. **Reddit Dataset**: CSV file with posts from monitored subreddits about AI-related discussions.
2. **Semantic Scholar Dataset**: CSV file containing metadata for research papers on various AI topics.
3. **Wikipedia Dataset**: CSV file with daily pageviews and metadata for AI-related Wikipedia pages
4. **Plots & Visualizations:** - all html and png files - plots from datasets analysis to discover AI trends. 
