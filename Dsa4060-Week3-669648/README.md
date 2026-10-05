# DSA4060-Week3-669648

**Course:** DSA 4060 – Recommender Systems
**Lab:** Week 3 Practical Lab – Building a Simple Content-Based Recommender
**Student ID:** 669648

## Overview
A simple content-based movie recommender built with pandas. Movies are described by five binary genre features (Action, Comedy, Drama, Romance, SciFi). A user profile is built from the user's ratings, every movie is scored against that profile, watched movies are removed, and the Top-N movies are returned.

Workflow: Movie Features → User Preferences → Recommendation Scores → Top Recommendations

## Repository contents
```
DSA4060-Week3-669648/
├── content_based_lab.ipynb
├── movies.csv
└── README.md
```
- `content_based_lab.ipynb` – the full lab, with explanations and outputs
- `movies.csv` – the 11-movie dataset (10 given movies + my unique movie, *Safari Heist*)
- `README.md` – this file

## How to run
1. Install the requirements: `pip install pandas jupyter`
2. Open the notebook: `jupyter notebook content_based_lab.ipynb`
3. Run all cells from top to bottom (Kernel → Restart & Run All).

## What the notebook covers
- Dataset exploration and the item-feature matrix
- Building a user profile by weighting features with ratings, then normalizing it
- Scoring, ranking, removing watched movies and generating Top-N recommendations
- A reusable `recommend_movies()` function
- Testing a second user (User B) and a thinking exercise on User C
- Adding my own movie (*Safari Heist*, Action + Comedy) and my own user
- Interpretation, limitations, conclusion and the final question

## Limitations (summary)
Only five genre features are used, other metadata is ignored, recommendations can be too similar to what the user already likes, new users have little history, and movies with identical profiles tie. TF-IDF and cosine similarity are covered in Week 4.
