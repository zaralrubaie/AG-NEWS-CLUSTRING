# AG News Clustering with TF-IDF + KMeans
## Project Overview
This project demonstrates how to cluster news articles into topics using unsupervised learning. We use the AG News dataset and perform text preprocessing, TF-IDF vectorization, and KMeans clustering, followed by visualization and interpretation of results.

## Objective

- Group news articles into meaningful clusters (topics)
- Explore top terms in each cluster
- Predict the topic of a new, unseen article

## kills & Technologies

- Python
- Pandas (data handling)
- NLTK (text preprocessing)
- Scikit-learn (TF-IDF, KMeans, PCA)
- Matplotlib (visualization)
-Unsupervised Learning (clustering)
- Natural Language Processing (NLP)

 ## Project Steps (Summary)
 
- Load & Prepare Data – Combine Title and Description into a single text column.
- Clean Text – Lowercase, remove special characters, numbers, and stopwords.
- Vectorize – Convert text into TF-IDF vectors.
- Cluster Articles – Apply KMeans to group articles into 4 clusters.
- Visualize & Interpret – Use PCA for 2D plotting and extract top terms per cluster.
- Predict New Articles – Clean, vectorize, and assign a topic to unseen text.

  ## Example output
  
 ````
Cluster 0 top terms: game, team, season, win, player, match, coach, league, points, cup
Cluster 1 top terms: government, president, election, country, policy, leader, minister, party, law, state
Cluster 2 top terms: company, market, business, stock, financial, report, growth, investors, revenue, shares
Cluster 3 top terms: trade, oil, commodity, energy, prices, industry, market, production, demand, export
````
### Predicted topic for a new article:
- Article: "Microsoft launches new AI-powered game console next month"
- Predicted cluster: 0
- Predicted topic: Sports
## How to Run
1. Clone this repository:
````
git clone <(https://github.com/zaralrubaie/AG-NEWS-CLUSTRING/edit/main/README.md)>
````
2. Install dependencies:
````
!pip install pandas scikit-learn matplotlib nltk
````
3. Download NLTK stopwords (once):
````
import nltk
nltk.download('stopwords')
````
4. Run the notebook (.ipynb) or Python script.
   
## Future Improvements

- Use word embeddings (e.g., Word2Vec, BERT) for better semantic understanding
- Experiment with different clustering algorithms (HDBSCAN, DBSCAN)
- Evaluate cluster quality using metrics like Silhouette Score
- Automatically assign topics using topic modeling (LDA or BERTopic)
