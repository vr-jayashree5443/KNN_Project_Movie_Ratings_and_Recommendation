# KNN_Project_Movie_Ratings_and_Recommendation

This project aims to analyze movie data, predict movie ratings, and provide movie recommendations using the K-Nearest Neighbors (KNN) algorithm. The dataset used in this project contains information about movies, including features such as budget, genres, keywords, popularity, revenue, runtime, release date, cast, and crew.

## Steps

1. **Import Libraries**: The necessary libraries for data analysis and machine learning tasks are imported.
2. **Import the Dataset**: Two datasets are imported: `tmdb_5000_movies.csv` and `tmdb_5000_credits.csv`, which contain information about movies and their credits respectively.
3. **Data Analysis**: Data Exploration (DE), Data Manipulation (DM), Data Cleaning (DC), Data Visualization (DV), and Exploratory Data Analysis (EDA) are performed to understand the dataset and its characteristics.
4. **[Optional] Hyperparameter Tuning**: Hyperparameters of the KNN model can be tuned for better performance.
5. **Feature Engineering**: Features are preprocessed and engineered for model input. This includes encoding categorical variables and feature scaling.
6. **Split the Data**: The dataset is split into training and testing sets using cross-validation.
7. **Model Selection**: The KNN algorithm is chosen as the model for predicting movie ratings.
8. **Training the Model**: The KNN model is trained using the training dataset.
9. **Test the Model**: The trained model is tested using the testing dataset.
10. **Performance Evaluation**: The performance of the model is evaluated using metrics such as confusion matrix and accuracy score.

## Dataset Information

The dataset consists of two main files:

1. **Movies Dataset**: Contains information about various movies, including their titles, genres, keywords, popularity, budget, revenue, runtime, release date, and more.

2. **Credits Dataset**: Provides details about the credits associated with each movie, including the cast and crew members.

Both datasets are merged based on the movie ID to consolidate all relevant information into a single dataframe.

## Data Cleaning and Preprocessing

The following preprocessing steps are performed on the dataset:

- Handling missing values: Columns with significant null values, such as `homepage` and `tagline`, are dropped. Rows with missing values in essential columns like `runtime` and `release_date` are removed.
- Date Parsing: The `release_date` column is split into separate columns for year, month, and day.
- JSON Parsing: Columns containing JSON data, such as `genres`, `keywords`, `production_companies`, `production_countries`, and `spoken_languages`, are parsed to extract relevant information.
- Crew Data Extraction: The `crew` column is processed to extract the names of directors and their respective departments.

## Feature Selection

For movie rating prediction, the following features are considered:

- Budget
- Genres
- Keywords
- Popularity
- Revenue
- Runtime
- Release date (Year, Month, Day)
- Cast
- Director

## Conclusion

This project demonstrates the process of analyzing movie data, predicting movie ratings, and providing recommendations using machine learning techniques. The KNN algorithm serves as a baseline model for predicting movie ratings based on various features. Further enhancements, such as incorporating more sophisticated algorithms or additional features, can be explored to improve the accuracy of predictions and recommendations.

