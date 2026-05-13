# CPSC 393 Machine Learning: Spotify Recommendation System
Machine learning-based music recommendation system using Spotify audio features and unsupervised models including KNN, K-Means, and DBSCAN.

**Created by:** [@amperry01](https://github.com/amperry01) and [@brookeengland](https://github.com/brookeengland)

## Project Overview
This project explores similarity-based music recommendation using Spotify audio features. We compare multiple unsupervised learning approaches to determine how well numerical audio features capture perceived musical similarity.

The project evaluates:
- KNN with Euclidean distance
- KNN with cosine similarity
- K-Means clustering
- DBSCAN clustering

## Setup Instructions
### Required Libraries
Install the following python libraries:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

The project was developed using:
- Python3
- Google Colab

All experiments and visualizations can be run directly in Google Colab.

## Dataset Information
**Dataset:** Spotify Audio Features dataset from Kaggle.

Approximate size:
- ~114,000 songs
- Numerical audio features and metadata

**Features used include:**
- danceability
- energy
- tempo
- loudness
- valence
- acousticness
- instrumentalness
- speechiness

The dataset can be downloaded from Kaggle using the link below. After downloading, upload the CSV file to Google Colab or update the dataset file path in the notebook before running the project.

**Dataset link:** [Kaggle Spotify Dataset](https://www.kaggle.com/datasets/vatsalmavani/spotify-dataset?select=data)

## How to Run the Code
1. Clone or download this repository.
2. Download the Spotify Audio Features dataset from Kaggle.
3. Upload the dataset to Google Colab or update the dataset file path in the notebook.
4. Open spotify_recommender.ipynb in Google Colab.
5. Run all cells in order from top to bottom.

The notebook includes:
- data preprocessing
- exploratory data analysis
- PCA visualizations
- KNN recommendation models
- K-Means clustering
- DBSCAN clustering
- evaluation and comparison results

## Results
Key findings from the project include:
- KNN models produced the most consistent recommendation behavior.
- Cosine similarity generated tighter local similarity groupings than Euclidean distance.
- K-Means produced weak and overlapping clusters in feature space.
- DBSCAN identified many noise points and struggled to form meaningful density-based clusters.
- PCA visualizations showed that the Spotify audio features do not naturally separate into distinct musical groups.

Overall, the project demonstrated that low-level Spotify audio features can capture numerical similarity between songs, but do not always align with human perception of musical similarity.

## Contributors
- **Alyssa Perry**  
AI/ML Intern @ The Aerospace Corporation | CS Student @ Chapman | [LinkedIn](https://linkedin.com/in/alyssamperry)

- **Brooke England**  
Data Science Student @ Chapman | [LinkedIn](https://www.linkedin.com/in/brooke-england-998584265/)
