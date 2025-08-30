# MovieAnalysis
## Scenario & Introduction
### Problem Statement\
Streaming platforms ingest hundreds of new titles every month, yet most arrive with only minimal metadata.
Without reliable genre tags or similarity links, users struggle to discover relevant content, and providers miss out on engagement opportunities.
### Business / Research Goal
Our goal is to **automatically enrich newly ingested movies** by providing:
1. **Primary genre predictions** derived solely from a plot summary.
2. **Content-based recommendations** that surface semantically similar titles on day 0.
#### Concrete Research Questions\n",
| #   | Question |
|-----|----------|
| **RQ-1** | *How accurately can genres be inferred from plot texts, and which model performs best?* |
| **RQ-2** | *Which text-representation strategy (e.g., TF-IDF, Word2Vec, Sentence-BERT) yields the best performance for the recommendation system?* |
### Strategy & Methodology
Our workflow is organised in **four notebooks**, each mapping to a specific project phase:
| Phase / Notebook | Key actions |
|------------------|-------------|
| **DataExtraction & Preprocessing** | • Download TMDB metadata and Wikipedia plots<br>• Normalise titles, merge datasets, remove duplicates |
| **DataExploration**  | • Inspect class balance, text length, language distribution<br>• Visualise token counts & top n-grams |
| **GenreClassification** | • Train and compare models: Logistic Regression, SVM, Random Forest, LSTM, BERT |
| **RecommenderSystem** | • Experiment with TF-IDF, Word2Vec, Sentence-BERT embeddings<br>• Retrieve neighbours via cosine similarity & HNSW |
