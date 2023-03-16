# Movielens Recommendation System

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
GroupLens, a resaerch lab at the University of Minnesota made available thee MovieLens dataset. The dataset has been used in various academic publications and competitions, which further validates its credibility. GroupLens is a reputable source for research in the field of recommendation system.    

# 5.Data Preprocessing
The data was individually checked for null values and for duplicates in the data. The datatypes of each of their columns was checked. Different tables were merged and their contents also checked for null values and for duplicates. Columns that were not important were dropped like the timestamp column. 

# 6.Exploratory Data Analysis
EDA showed interesting insights about our dataset MovieLens. we discovered that the most number of ratings from plotting a countplot for count of ratings, were rated four out of five. We also observed that the distribution of the release year was at peak from the 1990s through 2000s. Additionally, we found out that the overall ratings of movies produced in the earlier was lower, we found out about this by plotting a correlation of the release year and ratings.
## a)Univariate Analysis
This graph shows the number of movies per genre.

![1stImage](https://user-images.githubusercontent.com/117269915/225694368-da46d6f6-f685-4adf-81aa-e3ffa9877ed7.png)

The graph below shos the count of a given rating and four(4) is where most movies are rated.

![CountRating](https://user-images.githubusercontent.com/117269915/225694944-ef845bf8-4dab-4a90-8b92-6875d5f250a4.png)



Below is a distribution plot of the movies produced across the years with a peak being around the 1990s.

![CountYear](https://user-images.githubusercontent.com/117269915/225695466-423037c3-5a84-4acb-a4fd-ab3400da47b2.png)


## b)Bivariate Analysis
This graph shows the movie ratings across the years.The years were binned into bins of 10 years. From the previous insight we could conclude that the rating is low in earlier years as a result of less movies being produced during the same time.Also the 1990-2000 show an increace in the number of ratings.

![RatingYearBin](https://user-images.githubusercontent.com/117269915/225706100-9125dccb-bbb2-4ce5-b873-2ddc16c15429.png)



# 7.Modelling
## a. The popularity based baseline model 
With the assumption that some users that will use this system will be new , a model had to be created to accommodate users with no preference information.
*  If no information is provided, the user was recommended the popular movies which have been rated at least 150 times.
*  If the user presents a threshold, say, top 10, then the user gets the top 10 movies with highest ratings.
*  If the user presents a genre, then the user is recommended top-rated movies from that genre.
## b. The Collaborative Filtering Model
The collaborative filtering system leverages a user's watching history and the ratings they gave to those movies. 
It then recommends 5 movies they are most likely to want to watch
## c. The Hybrid model 
Finally, we combined the popularity-based model with the collaborative filtering model to get a hybrid that utilizes the functionality of both models. 
New users will get a recommendation of the top 5 popular movies, while an old user will get a list of 5 films they will most likely watch. 
## Model Selection




# 8.Conclusions
We have successfully built a movie recommender system using collaborative filtering that provides personalized movie recommendations to users. Our model has a low RMSE score and high recall score, indicating that it provides accurate and relevant recommendations to users. The MovieLens dataset provided a good foundation for building a movie recommender system.
1. Drama genre has the highest count with 41928 while Film Noir has the least with 870.
2. The analysis showed that most movies in the dataset received high ratings, with over 50% of movies rated between 4 and 5 stars.
3. Additionally, the majority of ratings were made between 1990 to 2000. The top three genres were drama, comedy, and action. Interestingly, the average rating of    movies watched by fewer people was higher than those watched by more people.
4. The analysis showed a positive correlation between the number of ratings and the average rating of movies. These findings could be useful to movie studios and streaming services to understand the trends and preferences of movie viewers and make informed decisions on which movies to produce and distribute.

# 9.Recommendations
We recommend the following to improve the movie recommender system:
1.	Include user demographics and movie metadata to provide even more personalized recommendations to users.
2.	Implement A/B testing to validate the effectiveness of the model and to ensure that it provides the desired impact on user satisfaction, engagement, and retention.
3.	Continuously update and improve the model to ensure that it stays relevant and up-to-date with users' changing preferences.
4.	Collaborate with other movie streaming platforms to increase the dataset size and diversity, which can enhance the model's performance and accuracy.
