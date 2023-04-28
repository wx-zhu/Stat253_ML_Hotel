# Predicting Hotel Reviewers’Scores for European Hotels

## About The Project
In this project, we used multiple machine learning tools in R to predict hotel reviewers’ score and understand what are some important aspects could impact the reviewers' score for European hotels. 

### Installation
Please fork this repository and open the repo in R to check out our R code. Or you can simply check out deployed web with code: https://hotel-review-ml.netlify.app/


## Machine Learning details
### Data Contect
The data we use in this project is originally owned by Booking.com, but we used the version from kaggle.com https://www.kaggle.com/jiashenliu/515k-hotel-reviews-data-in-europe

The dataset contains ~515,000 entries which are each customer reviews score 1493 different luxury hotels across Europe. Variables we use include reviewer’s negative/positive words, total review counts, reviewers’ nationality, time, hotel address, average score, etc.

### Data Cleaning

We use string detect and regular expression to clean data for country, and extract review year to allow a more generalized predicting. We also create season, reviewers' score and hotel average score difference (one categorical variable for logistic model and one quantitative variable for regression model), delete unnecessary columns 

### Research Questions
- Regression: We are interested in predicting how much the reviewer’s score differs from the average score of the hotel.

- Logistic: We are interested in predicting if the reviewer’s score would be above or below the average score of the hotel. 

- Clustering: We decided to use k-means clustering to further explore the relationship between reviewers’ score and how much positive & negative words they have in their review. (there is a very cool 3D plot in this session)

### Machine Learning Process

Check out deployed web with code: https://hotel-review-ml.netlify.app/

### Evaluation
Our ultimate goal is to understand what are some aspects could impact the review score for European hotels using machine learning tools. From multiple machine learning process, we find out that the number of positive and negative words in the review impact the review score the most. We are also able to predict the numeric difference in reviewers' score and hotels' average score using different tools in regression models. Other influnece includes reviewer’s nationality (continent in general), reviewers’ general behavior (do they write a lot reviews in general), season (holiday season or not). Future investigations could be study similar dataset from other continents: Asia, Africa, South America... or create tags for data mining and cluster words.

