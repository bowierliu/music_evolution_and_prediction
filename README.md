# Analyzing Musical Evolution and Predicting Song Virality in Pop Music

## Overview
This project aims to analyze the evolution of pop music and predict the virality of songs based on their audio features. Using Spotify's API, we collected data on various pop songs and employed both supervised and unsupervised learning techniques to understand trends and make predictions. This dual approach provides insights into historical trends and future virality, offering artists valuable tools for creating hit songs.

## Table of ContentS
1. [Introduction](#introduction)
2. [Related Work](#related-work)
3. [Data Source](#data-source)
4. [Feature Engineering](#feature-engineering)
5. [Supervised Learning](#supervised-learning)
6. [Unsupervised Learning](#unsupervised-learning)
7. [Results and Discussion](#results-and-discussion)
8. [Future Work](#future-work)
9. [Ethical Considerations](#ethical-considerations)
10. [Authors](#authors)
11. [License](#license)

## Introduction
Pop music is characterized by catchy melodies and widespread appeal, dominating charts and social media. Understanding the elements that drive a pop song to virality and analyzing evolutionary trends within the genre is crucial for artists. This project tackles two main challenges: identifying changing patterns in audio features over time and predicting which songs will go viral.

## Related Work
1. **Spotify for Artists**: Provides detailed analytics but lacks insights on audio features and genre evolution.
2. **Solving Spotify Multiclass Genre Classification Problem**: Focuses on genre classification rather than analyzing evolution within a genre.
3. **Predicting Song Popularity from Spotify Dataset (Kaggle)**: Uses regression for predicting popularity; our project employs classification to determine hit songs and is applicable to various artists.

## Data Source
Data was collected from Spotify API and an additional dataset from Kaggle. The final dataset contains approximately 2,500 records with features such as danceability, energy, key, loudness, mode, acousticness, instrumentalness, liveness, valence, tempo, duration, and explicitness.

## Feature Engineering
Key features were extracted, normalized, and missing values filled. The target variable "Virality" was created, labeling tracks with a popularity score above 80 as viral.

## Supervised Learning
Four classifiers were used:
- **Logistic Regression**
- **Random Forest**
- **K-Neighbors**
- **Support Vector Machine**

The best model was the Random Forest classifier, evaluated based on F1, Accuracy, and ROC-AUC scores.

## Unsupervised Learning
Clustering was performed using t-SNE with K-means to analyze pop music evolution. Clusters were compared across different decades to identify shifts in musical styles.

## Results and Discussion
- **Supervised Learning**: The Random Forest model achieved the highest performance with key features including valence, explicit, acousticness, and energy.
- **Unsupervised Learning**: Identified three primary clusters: Electropop, Dance Pop, and Acoustic Pop, each with distinct audio features. Notable trends in pop music evolution were observed, such as increased danceability and shorter song durations.

## Future Work
Future improvements could include incorporating lyrical content analysis using NLP techniques, experimenting with more clustering algorithms, and conducting a more granular temporal analysis.

## Ethical Considerations
Ethical considerations include potential biases in the dataset and the misuse of clustering results. Efforts were made to ensure a comprehensive representation of pop music over time and to educate stakeholders on the appropriate use of the results.

## Authors
- Andre Onofre
- Bowie Liu
