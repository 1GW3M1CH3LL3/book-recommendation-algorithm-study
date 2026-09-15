# A Comparative Study of Book Recommendation Algorithms

This project investigates how different recommendation methods compare in their ability to provide accurate and relevant personalized book recommendations.

## Project Overview

The project uses the Book-Crossing dataset to explore and compare two recommendation approaches:

- Content-based filtering
- Collaborative filtering

The content-based approach uses book metadata with TF-IDF and cosine similarity to identify similar books. The collaborative-filtering approach uses user-book rating patterns and SVD.

## Current Progress

- Prepared and cleaned the Book-Crossing dataset
- Performed exploratory data analysis
- Created an 80/20 training and testing split
- Implemented a content-based recommendation pipeline using TF-IDF and cosine similarity
- Generated top-5 personalized book recommendations
- Performed an initial Hit Rate@5 evaluation
- Implemented an initial SVD collaborative-filtering model and RMSE evaluation

## Next Steps

- Define relevant recommendations based on user ratings
- Implement Precision@5 and Recall@5
- Improve the evaluation procedure
- Compare content-based and collaborative-filtering performance
- Analyze the strengths and limitations of each approach

