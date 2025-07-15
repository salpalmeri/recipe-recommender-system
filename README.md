# Recipe Recommender System

This project implements multiple recommendation system techniques to suggest recipes based on user preferences and recipe attributes. It includes:

- Content Based Filtering
- Collaborative Based Filtering
- Hybrid Recommender System (Content + Collaborative)

---

## Dataset Overview

The system uses two datasets:
- 'recipes': Contains recipe data such as name, ingredients, steps, tags, etc.
- 'interactions': Includes user interaction data such as user ID, recipe ID, rating, etc.

---

## Tools

- Jupyter Notebook
- Libraries:
  - 'pandas', 'numpy'
  - 'scikit-learn' for modeling and vectorization
  - 'TfidVectorizer', 'cosine_similarity', 'KNN' for similarity scoring
 
---

## Recommendation Techniques

### 1. Content Based Filtering
- Uses 'TfidVectorizer' to compute similarity between recipes based on features like recipe name, steps, and ingredients.
- Gives recommendations based on similar recipes to the given one.

### 2. Collaborative Filtering
- Builds user item matrix from the interactions dataset.
- Applies 'KNN' to find similar users and recommend recipes they liked.

### 3. Hybrid Recommender
- Combines content similarity and collaborative scores.
- Uses recipe similarity with user history for better results.

---

## Sample Outputs

### Content Based:
Recipe: 'beef in red wine mushroom sauce'
Suggested:
- 'red wine and garlic mushrooms'
- 'catfish fillets in white wine and mushroom sauce'

### Collaborative Filtering:
For 'user_id = 126440', recommended:
- 'aioli with herbs'
- 'garlic and mushroom soup'
- 'cranberries in red wine'

### Hybrid System:
for 'user_id = 126440' and recipe: 'beef in red wine mushroom sauce'
Combined recommendation output:
- 'beef enchiladas with red sauce'
- 'red wine and garlic mushrooms'
- catfish fillets in white wine and mushroom sauce'

---
