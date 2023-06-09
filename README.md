# Book Rating Prediction using Recommender Systems
## Project Description
<p align="justify">
The goal of the project is to build a recommender system for books. For this exercise, we have used the dataset containing books related to the genre “Poetry” from Goodreads. In this project, we have implemented a recommendation
system, for recommending poetry books using multiple approaches based on collaborative filtering and other models leveraging deep learning methods. We've used three implementations, item-item collaborative filtering, neural collaborative filtering as well as wide-and-deep model for recommender systems.

The [dataset](https://sites.google.com/eng.ucsd.edu/ucsdbookgraph/home) used for this project comes from the book cataloging website Goodreads, and it has data on over 36K books and 377K users.</p>

<p align="justify">
We have evaluated and compared the results obtained from each model. Our first approach, which serves as a baseline for the remaining models, is Item-Item Collaborative Filtering. Here, we directly used the ratings given by users for different books for predicting user ratings. We later improved upon the predictions obtained from this model by generating embeddings for users and items using Matrix Factorization, and then later trained MLP and NeuMF for predicting the final rating given by a user for a particular book. The summary of the Model results is as follows:
</p>

|Model|MAE|MSE|
|-----|---|---|
|Item-Item Collaborative Filtering| 2.851| 11.518|
|NCF with Matrix Factorization| 0.97| 1.426|
|Neural Matrix Factorization (NeuMF) |0.784 |1.002|
|NeuMF with Book Genres |0.779| 0.964|
|Wide-and-Deep Recommendation Model| 0.717| 0.774|

<p align="justify">
The Wide-and-Deep model approach gave us the lowest Mean Squared Absolute error, marginally better than NCF models and significantly improved over Item-Item CF.</p>
