# Movie Recommender System

## Overview
In our Business Analytics Master's program at Nova School of Business and Economics, my team and I completed a class project for our "Machine Learning" course. We developed a movie recommendation system using a Kaggle dataset with Metadata on over 45,000 movies and 26 million ratings from over 270,000 users:

https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset/code?datasetId=3405&sortBy=voteCount

Recommendation systems are crucial today for enhancing user experience and engagement. They offer personalized suggestions, boosting satisfaction and retention while driving sales and loyalty across digital platforms like streaming services. In our case, we developed recommender systems for a fictional customer to simulate a real-world scenario.

The project had two phases: the first involved traditional Machine Learning techniques, while the second focused on enhancing our recommendation system with Deep Learning methods. After testing several models, we combined Content-Based and Collaborative Filtering techniques to maximize the relevance of our recommendations:
- Content-Based Recommender Systems provide immediate personalization since they do not require ratings to begin generating recommendations. This makes them particularly robust and effective at mitigating the cold start problem. Ultimately, we integrated **Word2Vec text embeddings with BERT-based sentiment analysis**, achieving a **precision of 80.74%**, meaning that out of 10 suggested movies, at least 8 are relevant for the user.
- Additionally, we implemented a Collaborative Filtering model that leverages user behavior and interactions to suggest movies liked by similar users, further enhancing personalization and relevance. For this, we used a **Neural Collaborative Filtering (NCF)** model, which combines Generalized Matrix Factorization and Multi-Layer Perceptron to learn complex user-item interactions. This model achieved a **precision of 98.39%** and an **RMSE of 1.05** (on a rating scale of 0.5 to 5).

[Content Based Models - Overview](additionalContent/Content_Based_Models_Overview.png)

[Collaboreative Filtering Models - Overview](additionalContent/Collaborative_Filtering_Models_Overview.png)

## Repository Structure
**data:**
The directory where the Kaggle data files should be placed.

**notebooks:**
This includes the Notebooks from both parts of the project.

## How to Use
**Installation:**
1. Clone the repository:
```sh
    git clone https://github.com/xxnado/Movie-Recommender-System.git 
    cd Movie-Recommendation-System
```
2. Install the required libraries:
```sh
    pip install -r requirements.txt
```
3. Download the dataset from Kaggle and put it in the `data/` directory.

**Running the Notebooks:**
1. Open Jupyter Notebook:
```sh
jupyter notebook
```

2. Run the notebooks `Part1_Master_Notebook.ipynb` and `Part1_Master_Notebook.ipynb`.

## Authors
Students who developed this project (in alphabetical order):
- Benedikt Tremmel
- Gilian Wagner
- Leonardo Heinemann
- Malte Haupt
- Maximilian Schön
