# CSL7110 Assignment 3 – Recommender Systems

Implementation of Assignment 3 for **CSL7110 – Machine Learning with Big Data**.
Covers 13 recommender system tasks using the **MovieLens dataset**, from basic content-based filtering to neural networks, reinforcement learning, and explainability.

## Course Details

| Field | Details |
|-------|---------|
| Course | CSL7110 – Machine Learning with Big Data |
| Assignment | Assignment 3 |
| Student | Akshay Kumar |
| Student ID | M25DE1028 |
| Dataset | MovieLens (movies.csv, ratings.csv) |

---

## What Was Built

### Part 1 – Content-Based Filtering
- **Task 1:** TF-IDF Based Recommendation — genre vectors + cosine similarity
- **Task 2:** User-Profile CBF — weighted user profiles + Precision@K / Recall@K evaluation

### Part 2 – Collaborative Filtering
- **Task 3:** User-Based CF — Pearson correlation, multiple K values, RMSE + Precision@K
- **Task 4:** Item-Based CF — item-item similarity, comparison with user-based CF

### Part 3 – Matrix Factorization
- **Task 5:** SVD from scratch — numpy/scipy, latent factor analysis
- **Task 6:** Surprise SVD — hyperparameter tuning with GridSearchCV, comparison with Task 5

### Part 4 – Hybrid Model
- **Task 7:** Hybrid Meta-Model — Gradient Boosting to blend CBF + CF scores, cold-start analysis

### Part 5 – Learning-Based
- **Task 8:** Neural Network CBF — MLP with user and movie feature embeddings
- **Task 9:** Reinforcement Learning — ε-Greedy MAB, UCB, and Q-Learning agents

### Part 6 – Explainability
- **Task 10:** SHAP — feature importance for the hybrid model
- **Task 11:** Neighbourhood-Based — explains which similar users/items drove recommendations
- **Task 12:** LIME — local explanations for the neural network
- **Task 13:** Explainability Evaluation — consistency, coverage, and bias detection

---

## Evaluation Metrics Used

- RMSE (Root Mean Squared Error)
- Precision@K and Recall@K
- Cumulative reward (RL tasks)
- SHAP / LIME feature weights (explainability tasks)

---

## How to Run

1. Clone the repo and navigate to the project folder
2. Create and activate the virtual environment:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the notebook:
   ```bash
   jupyter notebook Assignmnet3_Recommender.ipynb
   ```
4. Run **Kernel → Restart & Run All** to execute all 13 tasks in order

> **Note:** Tasks 7 onwards may take 1–2 minutes each due to model training. All tasks are optimised to run on the full dataset without excessive wait times.

---

## Dependencies

Key packages used (see `requirements.txt` for full list):

- `pandas`, `numpy`, `scipy`
- `scikit-learn` — TF-IDF, MLP, evaluation
- `scikit-surprise` — CF and SVD models
- `shap` — feature-based explainability
- `lime` — model-agnostic explainability
- `matplotlib`, `seaborn` — visualisations

---

## Project Structure

```text
CSL7110_Assignment3_RecommenderSystems/
│
├── Assignmnet3_Recommender.ipynb   ← main notebook (all 13 tasks)
├── M25DE1028_CSL7110_Assignment3.docx  ← report
├── requirements.txt
├── README.md
└── dataset/
    ├── movies.csv
    └── ratings.csv
```
