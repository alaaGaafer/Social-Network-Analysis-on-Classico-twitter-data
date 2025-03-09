# Social Network Analysis on Twitter Data

## Overview
This project performs Social Network Analysis (SNA) on a dataset of tweets related to "El Clasico." It constructs a graph based on tweet similarity and applies various graph analysis techniques, including k-core, k-truss, and k-clique to identify communities within the dataset.

## Features
- **Data Preprocessing:** Cleans and structures tweet data from a text file.
- **Text Similarity Analysis:** Uses TF-IDF vectorization and cosine similarity to measure tweet similarity.
- **Graph Construction:** Builds a weighted graph using tweet similarity and temporal proximity.
- **K-Core Analysis:** Identifies highly connected nodes by extracting k-core subgraphs.
- **K-Truss Analysis:** Further refines the k-core by enforcing triangle connectivity.
- **K-Clique Analysis:** Detects dense communities using the k-clique percolation method.
- **Community Detection:** Extracts and labels different communities from the graph.
- **Visualization:** Uses NetworkX and Matplotlib to visualize the constructed networks.

## Dependencies
Ensure you have the following Python libraries installed:
```bash
pip install pandas networkx scikit-learn matplotlib
```

## Data
The dataset consists of tweets related to "El Clasico," stored in `Clasico.txt` with the following structure:
- `TweetID`: Unique identifier for each tweet.
- `Tweet_Text`: Content of the tweet.
- `DateTime`: Timestamp of the tweet.
- `Location`: (Dropped during preprocessing)

## Usage
1. Load the dataset from `Clasico.txt`.
2. Compute TF-IDF-based text similarity and construct a weighted graph.
3. Apply graph analysis techniques (k-core, k-truss, k-clique) to extract communities.
4. Visualize the resulting network graphs.

## Results
- A network graph representing tweet relationships.
- Extracted communities based on different graph-theoretic techniques.
- Insights into the structure of Twitter interactions related to "El Clasico."

