# CSL7110 Assignment 3 – Recommender Systems

This repository contains the implementation of Assignment 3 for the course **Machine Learning with Big Data**.  
The work focuses on building and comparing different recommender system techniques using the **MovieLens dataset**.

## Course Details
- **Course:** CSL7110 – Machine Learning with Big Data
- **Assignment:** Assignment 3
- **Student Name:** Akshay Kumar
- **Dataset Used:** MovieLens

## Objective
The main objective of this assignment is to understand and implement different recommendation approaches, including content-based filtering and collaborative filtering, and to compare their performance.

## Implemented Tasks
The following recommender system methods were implemented in the notebook:

1. **TF-IDF Based Content Recommender**
   - Movie genres were converted into TF-IDF vectors
   - Cosine similarity was used to recommend similar movies

2. **User Profile Based Content Recommender**
   - User profiles were created using weighted averages of rated movie features
   - Personalized recommendations were generated

3. **User-Based Collaborative Filtering**
   - Similar users were identified using rating patterns
   - Recommendations were generated based on neighbors’ preferences

4. **Model-Based Collaborative Filtering using SVD**
   - Singular Value Decomposition (SVD) was used to learn latent user-item factors
   - Predicted ratings were used for recommendation

## Evaluation
The implemented models were evaluated using:
- **RMSE (Root Mean Squared Error)**
- Recommendation outputs for sample users and movies

## Dataset
This assignment uses the **MovieLens dataset** provided by GroupLens.

Files used:
- `movies.csv`
- `ratings.csv`

## Project Structure
```text
CSL7110_Assignment3_RecommenderSystems/
│
├── Assignmnet3_Recommender.ipynb
├── M25DE1028_CSL7110_Assignment3.docx
├── README.md
├── .gitignore
└── dataset/
    ├── movies.csv
    └── ratings.csv