# Book-Recommendation-Engine

Dataset Link :- https://drive.google.com/drive/folders/1EcTYayw8UkbojgQSH3a2nkqePn8cz4KY?usp=sharing

## Performing EDA on Dataset:-

### 1. Age distribution of users:
![Age_Distribution](https://user-images.githubusercontent.com/29835510/137723212-0f21610e-84b7-4a19-a213-e1fb0c452837.PNG)

Here, The most active users are among those in their 20–30s.

### 2. Outliers Detection:
![outlier_detection](https://user-images.githubusercontent.com/29835510/137723355-7a68bca3-d7e2-4b0e-9576-8539273f107c.PNG)

Age : 244
Ok we have Outlier data in Age

### 3. Users Country wise
![most_user_country](https://user-images.githubusercontent.com/29835510/137723526-c4dad08c-74ac-4761-9105-eb941f9bb6bf.PNG)

Most number of users are from USA

### 4. Top 10 Authors
![top10user](https://user-images.githubusercontent.com/29835510/137723625-536de024-09a3-453b-96a0-57d3d9ebddec.PNG)

### 5. Top 10 Publishers
![top10publisher](https://user-images.githubusercontent.com/29835510/137723704-98a23dbc-55e9-4fc3-aa20-6d9c0c278e25.PNG)

### 6. Rating Distributions
![Rating_distribution](https://user-images.githubusercontent.com/29835510/137723807-50dd6326-3f8d-4028-a4db-6f36619fd6bd.PNG)

The ratings are very unevenly distributed, and the vast majority of ratings are 0 .As quoted in the description of the dataset - BX-Book-Ratings contains the book rating information. Ratings are either explicit, expressed on a scale from 1-10 higher values denoting higher appreciation, or implicit, expressed by 0.

## Popularity Based Filtering
It basically uses the items which are in trend right now. For example, if any book which is usually bought by every new user then there are chances that it may suggest that book to the user who just signed up.

### Top Recoomendations of Popularity based filtering
![popularity based](https://user-images.githubusercontent.com/29835510/137724059-05b09dc2-48a8-4805-a7d6-112297a17652.PNG)

## Collaborative Filtering Recommender
## 1. Model Based:

Model based approach involves building machine learning algorithms to predict user's ratings. They involve dimensionality reduction methods that reduce high dimensional matrix containing abundant number of missing values with a much smaller matrix in lower-dimensional space.

### 1. Analysis of Collaborative Filtering model results
![model_based](https://user-images.githubusercontent.com/29835510/137724388-34a8d1d7-4ba9-4982-bdbe-adb750edb6a0.PNG)

Distribution of actual and predicted ratings in the test set According to the distribution of actual ratings of books in the test set, the biggest part of users give positive scores - between 7 and 10. The mode equals 8 but count of ratings 7, 9, 10 is also noticeable. The distribution of predicted ratings in the test set is visibly different. One more time, 8 is a mode but scores 7, 9 and 10 are clearly less frequent. It shows that the recommender system is not perfect and it cannot reflect the real distribution of book ratings.

### Graphical Representation:
![model_based1](https://user-images.githubusercontent.com/29835510/137724549-b5f2ce71-4c96-41e6-bbdb-52ba0aea90a3.PNG)

### 2. Absolute error of predicted ratings
![model_based2](https://user-images.githubusercontent.com/29835510/137724654-65a272bf-670c-470c-bb5f-9ca912e9bbf4.PNG)

The distribution of absolute errors is right-skewed, showing that the majority of errors is small: between 0 and 1. There is a long tail that indicates that there are several observations for which the absolute error was close to 10.

## 2. Memory Based:
## A. Item-Item Based Collaborative Filtering

### 1. Pivot Table
![matrix item-item](https://user-images.githubusercontent.com/29835510/137724894-08702a52-3529-4aae-b5f1-45079c690bae.PNG)

### 2. Recommendations
![sol item-item](https://user-images.githubusercontent.com/29835510/137724923-a4fb343a-2097-48d9-87c8-08fb595e7d7e.PNG)


## B. User-Item Based Collaborative Filtering

### 1. Pivot Table
![matrix user-item](https://user-images.githubusercontent.com/29835510/137725029-4e5ea012-2fca-48e8-9ff6-2e989c96ae33.PNG)

### 2. Recommendations
![sol user-item](https://user-images.githubusercontent.com/29835510/137725071-b74712fb-aa96-452f-af69-fada2fe79162.PNG)

