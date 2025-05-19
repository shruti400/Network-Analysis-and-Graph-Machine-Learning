News Article Summary Dataset

Dataset Description

This dataset contains information on 10,000 news articles, including their topics, the full text of the articles, and extractive summaries. It is designed for tasks related to natural language processing and graph-based analysis of text data.

File Contents

The dataset is provided as a single CSV file:

*   `synthetic_news_dataset_10k.csv`: Contains the data for 10,000 news articles.

Data Fields

The `synthetic_news_dataset_10k.csv` file contains the following fields:

*   `category`: The topic or category of the news article. Possible values include 'politics', 'crime', 'sports', and 'movies/entertainment'.
*   `text`: The full text of the news article.
*   `summary`: An extractive summary of the news article.

Purpose

This dataset can be used for various tasks, including:

*   Extractive Summarization:* Developing and evaluating methods to generate summaries by selecting key sentences from the original text, potentially using graph-based approaches like centrality measures.
*   Community Detection: Identifying groups of similar articles based on their content, which can be achieved by building a graph where nodes are articles and edges represent similarity.
*   Supervised Classification: Training models to classify news articles into their respective categories based on the article text or learned features.
*   Graph-Based Text Analysis: Exploring the application of graph theory and graph neural networks (GNNs) for understanding the structure and relationships within news content.

