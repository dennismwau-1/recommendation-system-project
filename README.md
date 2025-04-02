# Recommendation-System-Project
 ![Image Alt](https://github.com/dennismwau-1/recommendation-system-project/blob/15b8d6a61ba2697dfe643216c85e65b5fc09ea3e/poster.jpg)
Authors: dennis mwau,tabby mirara,justin mbugua,sharon momanyi,stephen munyiala
# INTRODUCTION
 “What movie should I watch this evening?”
 Have you ever had to answer this question at least once when you came home from 
work? As for me—yes, and more than once.
 This project aims to build a movie recommendation system by analyzing patterns in how 
users rate different movies, then suggesting the top 5 movies that a user is most likely to 
enjoy therefore increasing engagement for streaming platforms
# Data Overview
 This dataset utilizes information from IMDb and 
TMDb and describes 5-star rating and free-text 
tagging activity from MovieLens, a movie 
recommendation service. It contains 100,836 
ratings and 3,683 tag applications across 9742 
movies
# Project Objectives
 
 - Create a movie 
recommendation 
system.
 
 - Predict the rating that a 
user would give to a 
movie that he has not 
yet rated.
- Minimize the difference 
between predicted and 
actual rating (RMSE and 
MAE
# Exploratory Data Analysis
# Distribution of user rating count
![Image Alt](https://github.com/dennismwau-1/recommendation-system-project/blob/97d4a41122e3466d1a79537e098dee2e129bef55/distribution%20of%20user%20rating%20counts.PNG)
   
   We can see that most users rate 
very few movies, and few users 
rate many movies.
 This shows that the dataset has a 
lot of users with little interaction

![Image Alt](https://github.com/dennismwau-1/recommendation-system-project/blob/97d4a41122e3466d1a79537e098dee2e129bef55/distribution%20of%20user%20ratings.PNG)


From this plot, it is evident that, 
very many movies have few 
ratings while few movies have 
many ratings.
# Rating Distribution
![Image Alt](https://github.com/dennismwau-1/recommendation-system-project/blob/19281725497810eb2a17ba8019069f11195a4fc8/ratings%20distribution.PNG)

 Most movies recieve a rating of 4.0 
followed by 3.0. 
It is possible that users are generous 
with their ratings, giving a 3 if they 
don't really like a movie, 4 if the movie 
was alright and 5 if they really enjoyed 
the movie
# top 10 most rated movies 
![Image Alt](https://github.com/dennismwau-1/recommendation-system-project/blob/19281725497810eb2a17ba8019069f11195a4fc8/top%2010%20most%20rated%20movies.PNG)

 This graph shows the top 
10 most rated movies with 
Braveheart at the top.
# Frequency of each movie genre
![Image Alt](https://github.com/dennismwau-1/recommendation-system-project/blob/19281725497810eb2a17ba8019069f11195a4fc8/frequency%20of%20each%20movie%20genre.PNG)

Drama has the highest ratings 
followed by comedy while film-Noir 
has the least count of ratings
# Average Rating Per Genre
![Image Alt](https://github.com/dennismwau-1/recommendation-system-project/blob/19281725497810eb2a17ba8019069f11195a4fc8/avg.rating%20by%20genre.PNG)



 Film-Noir, War, and 
Documentary have the highest 
average ratings although they 
appear least frequently in the 
previous graph.

# Recommendation Models
 - Collaborative Filtering (SVD)
 This was used to recommendmovies based on 
user behaviour.
 - Content-Based Filtering
 This was used to compute the similarity between 
movies based on their genres. It allows us to 
recommend movies that share similar genre 
characteristics.
 - Hybrid Recommendation System
 This was used to improve recommendation quality, 
CF (SVD) is blended with CBF (genre similarity). 
This approach balances personalized predictions 
with genre- based similarities, helping address the 
cold start problem for new users
# Model Comparison
SVD performance: SVD consistently has a lower RMSE and MAE compared to the Hybrid system. This suggests that, in this 
particular evaluation, SVD is making more accurate predictions than the Hybrid approach.
 Hybrid Performance: The Hybrid system shows significantly higher RMSE and MAE. This indicates that its predictions are further 
away from the actual ratings than those of SVD
![Image Alt](https://github.com/dennismwau-1/recommendation-system-project/blob/e7073dc9fe3ad8daed191071bc3dd340a566f75c/model%20comparison.PNG)
# Error Distribution
![Image Alt](https://github.com/dennismwau-1/recommendation-system-project/blob/e7073dc9fe3ad8daed191071bc3dd340a566f75c/Error%20Distribution.PNG)


 The Hybrid Model appears to be biased negatively but appears to be more consistent and has lower error variance. Since 
the goal is to have errors closer to zero on average, the SVD model is more preferable but its spread suggests that it's 
inconsistent.
















