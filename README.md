# product-recommendation-system

The Product Recommendation System is a machine learning-driven project designed to offer personalized product suggestions to users based on their browsing and purchase history. By leveraging collaborative filtering and content-based filtering algorithms, the system analyzes user behavior to generate relevant recommendations, ultimately aiming to enhance the overall shopping experience and boost sales for e-commerce businesses.

Dataset

The project utilizes an Amazon dataset containing user ratings for electronic products. To maintain impartiality, each product and user is assigned a unique identifier rather than using personal information.

Approach

Rank-Based Product Recommendation:
Objective:

Recommend products with the highest number of ratings.
Target new customers with the most popular products.
Address the Cold Start Problem.
Outputs:

Recommend the top 5 products with a minimum of 50/100 ratings/interactions.
Approach:

Calculate the average rating for each product.
Determine the total number of ratings for each product.
Create a DataFrame and sort it based on the average rating.
Develop a function to retrieve the top 'n' products with a specified minimum number of interactions.
Similarity-based Collaborative Filtering:
Objective:

Provide personalized and relevant recommendations to users.
Outputs:

Recommend the top 5 products based on interactions of similar users.
Approach:

Convert user_id to integer type for ease of processing.
Develop a function to find similar users based on cosine similarity scores.
Write a function to recommend products based on interactions of similar users.
Model-based Collaborative Filtering:
Objective:

Provide personalized recommendations to users based on their past behavior and preferences.
Address challenges of sparsity and scalability.
Outputs:

Recommend the top 5 products for a particular user.
Approach:

Convert the matrix of product ratings to a compressed sparse row (CSR) matrix.
Perform singular value decomposition (SVD) to reduce dimensionality.
Calculate predicted ratings for all users using SVD.
Develop a function to recommend products based on rating predictions.
Evaluation:

Calculate the RMSE of the SVD model to evaluate its performance.
This project aims to offer tailored product recommendations, thereby improving user engagement and driving sales for e-commerce platforms.
