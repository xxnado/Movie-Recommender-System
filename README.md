# Movie Recommender System

## Overview
This project was developed as a class project for the "Machine Learning" course at Nova School of Business and Economics. The project involves movie recommendation systems, built on a Kaggle dataset with Metadata on over 45,000 movies and 26 million ratings from over 270,000 users:

https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset/code?datasetId=3405&sortBy=voteCount

Recommendation systems are crucial for enhancing user experience and engagement. They offer personalized suggestions, boosting satisfaction and retention while driving sales and loyalty across digital platforms like streaming services. In our case, the recommender system was developed for a fictional customer to simulate a real-world scenario.

The project had two phases: the first involved traditional Machine Learning techniques, while the second focused on enhancing the recommendation system with Deep Learning methods. After testing several models, Content-Based and Collaborative Filtering techniques where combined to maximize the relevance of the recommendations:
- Content-Based Recommender Systems provide immediate personalization since they do not require ratings to begin generating recommendations. This makes them particularly robust and effective at mitigating the cold start problem. Ultimately, **Word2Vec text embeddings with BERT-based sentiment analysis** where integrated, achieving a **precision of 80.74%**, meaning that out of 10 suggested movies, at least 8 are relevant for the user.
- Additionally, a Collaborative Filtering model that leverages user behaviour and interactions to suggest movies liked by similar users was integrated, further enhancing personalization and relevance. For this, a **Neural Collaborative Filtering (NCF)** model was used, which combines Generalized Matrix Factorization and Multi-Layer Perceptron to learn complex user-item interactions. This model achieved a **precision of 98.39%** and an **RMSE of 1.05** (on a rating scale of 0.5 to 5).

[Content Based Models - Overview](additionalContent/Content_Based_Models_Overview.png)

[Collaboreative Filtering Models - Overview](additionalContent/Collaborative_Filtering_Models_Overview.png)

## Repository Structure
**data:**
The directory where the Kaggle data files should be placed.

**notebooks:**
This includes the Notebooks from both parts of the project.

## How to Use
1. Clone the repository:
```sh
    git clone https://github.com/xxnado/Movie-Recommender-System.git 
    cd Movie-Recommender-System
```
2. Install the required libraries:
```sh
    pip install -r requirements.txt
```
3. Download the dataset from Kaggle and put it in the `data/` directory.

4. Run the Jupyter notebooks `Part1_Master_Notebook.ipynb` and `Part2_Master_Notebook.ipynb`.

## Authors
Students who developed this project (in alphabetical order):
- Benedikt Tremmel
- Gilian Wagner
- Leonardo Heinemann
- Malte Haupt
- Maximilian Schön
