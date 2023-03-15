# movielens Recommendation System

# 1.Business Understanding
## a)Analytical question
Ichigo is a movie company that wants to expand their horizons and make a recommender system called MovieLens based on collaborative filtering for thousands of their clients. The recommender system aims to improve user experience by offering personalized movie recommendations catering to each user's preferences. A better user experience, in turn, increases user satisfaction, engagement, and retention, thus increasing the profitability of the streaming platforms it serves. MovieLens has collected user ratings and movie watch history data on its platform to aid this research.

## b) Problem Statement: 
To build a model that provides top 5 movie recommendations to a user, based on their ratings of other movies.

## c) Defining the metric of success:
Having a model that has a low RMSE and a high recall score.
## d) Objectives
### Main objective
The main objective is to provide a valuable resource (Recommender system) for users to be able to enjoy a range of suggested similar movies based on product similarity or user similarity.

### Specific Objectives

1. To build and evaluate recommendation algorithms: This is meant to help  decide on the weaknesses and strengths of the algorithms and decide on the best.

2. To study user behavior: It will enhance the ability for the model to pick on the best predictions for the specified user.

3. To improve movie recommendations: By use of grid search for hyperparameter tuning that gives the optimal features that enable the algorithm to give as best predictions as possible.

4.  To test and validate new algorithms: The test ensures that our model is generalized,i.e it neither overfits or underfits.



# 3. Data Understanding
The MovieLens dataset contains 100,000 ratings, as well as demographic information and movie metadata, collected from 9,000 movies by 600 users. The dataset was collected and made available by GroupLens, a research lab at the University of Minnesota. The purpose of the dataset is to enable research in recommendation systems and related fields.

The dataset can be downloaded from the GroupLens website (https://grouplens.org/datasets/movielens/latest/).

On evaluation, our datasets meets all of the following requirements for preprocessing to take place smoothly.

1.Completeness-There are no missing values.

2.Consistency-as the individual features meet the required set of datatypes.

3.Validity-All the columns are independent and there is unique representations of the data points.

4.Accuracy-Based on the individual features representation,despite splitting the the genre column later on,the data is all accurate

# 4.External Data-source Validation


# 5.Data Preprocessing


# 6.Exploratory Data Analysis
## a)Univariate Analysis
This graph shows the number of movies per genre
![download](images/download.png)

The graph below shos the count of a given rating and four(4) is where most movies are rated
![download (1)](images/download (1).png)

Below is a distribution plot of the movies produced across the years with a peak being around the 1990s
[download (1)](images/download (1).png)

## b)Bivariate Analysis
This graph shows the movie ratings across the years.From the previous insight we could conclude that the rating is low in earlier years as a result of few produced movies during the same time.
[download (3)](images/download (3).png)

# 7.Modelling

# 8.Conclusions

# 9.Recommendations
