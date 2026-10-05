# A Comparative Study of Book Recommendation Algorithms

This project compares content-based filtering and collaborative filtering for personalized book recommendations using the Book-Crossing dataset.

## Research Question

**How do content-based filtering and collaborative filtering compare in top-N book recommendation performance under different levels of user-rating sparsity in the Book-Crossing dataset?**

## Recommendation Methods

### Content-Based Filtering
The content-based model uses available book metadata:
- Book title
- Author
- Publisher

TF-IDF is used to represent the metadata numerically, and cosine similarity is used to identify similar books.

### Collaborative Filtering
The collaborative filtering model uses Singular Value Decomposition (SVD) to learn patterns from explicit user-book ratings.

## Evaluation

The models are evaluated using:
- Precision@5
- Recall@5
- RMSE for SVD rating prediction

For the top-N evaluation, a relevant book is defined as a held-out test book with a rating of 7 or higher.

A controlled evaluation framework is used so that both recommendation approaches are compared using the same users, book catalog, relevance definition, and held-out test items.

## User-Rating Sparsity Experiment

The current experiment investigates recommendation performance when users have limited rating histories.

Both models are evaluated with:
- 1 available rating
- 2 available ratings
- 3 available ratings
- 4 available ratings

The experiment is repeated using five random seeds, and mean performance and standard deviation are calculated across the repetitions.

## Current Progress

- Prepared and cleaned the Book-Crossing dataset
- Implemented content-based filtering using TF-IDF and cosine similarity
- Implemented collaborative filtering using SVD
- Evaluated SVD rating prediction using RMSE
- Implemented Precision@5 and Recall@5
- Developed a controlled evaluation framework
- Checked the controlled data for test-book leakage
- Completed initial user-rating sparsity experiments
- Repeated sparsity experiments across five random seeds
- Generated comparison results and visualizations

## Preliminary Results

Across the tested sparsity levels, the content-based model achieved higher mean Recall@5 than SVD. However, performance did not consistently increase as additional user ratings became available.

These results are preliminary and apply to the current experimental setup. Further analysis and methodological refinement are planned.

## Next Steps

- Further analyze the sparsity experiment results
- Investigate improvements to the content-based user profile
- Examine whether the evaluation catalog can be expanded
- Refine result visualizations
- Document experimental limitations
- Complete the final comparative analysis and report
