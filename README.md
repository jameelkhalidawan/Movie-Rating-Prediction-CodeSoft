**Introduction**
Predicting IMDb movie ratings is a common task in the field of data science and machine learning. This script demonstrates how to build a predictive model for IMDb movie ratings using a Random Forest Regression model. The script includes data preprocessing steps, model training, hyperparameter tuning, evaluation, and visualization of the results.

**Requirements**
Before running the script, ensure you have the following dependencies installed:

Python (>= 3.6)
pandas
numpy
matplotlib
seaborn
scikit-learn

You can install these packages using pip:

**Copy code**
pip install pandas numpy matplotlib seaborn scikit-learn

**Getting Started**
Clone this repository to your local machine:

**Copy code**
git clone <repository-url>

Navigate to the project directory:
**Copy code**
cd imdb-movie-rating-prediction
**Run the script:**

Copy code
python imdb_rating_prediction.py

**Data**
The dataset used in this project is named "IMDB Movies India.csv." It contains information about various movies, including features such as the movie's name, release year, duration, director, actors, genre, and IMDb rating.

**Data Preprocessing**
The script performs the following preprocessing steps on the dataset:
Extracts the year from the 'Year' column and converts it to integers.
Converts the 'Duration' column to integers.
Uses one-hot encoding to split the 'Genre' column into binary variables.
Encodes categorical variables like 'Director,' 'Actor 1,' 'Actor 2,' and 'Actor 3' using Label Encoding.
Model Training and Hyperparameter Tuning
The script uses a Random Forest Regression model to predict IMDb movie ratings.
Hyperparameter tuning is performed using RandomizedSearchCV to find the best combination of hyperparameters.
The best model is selected based on the tuning results.
Evaluation
The model's performance is evaluated using the following metrics:
Mean Absolute Error (MAE)
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
R-squared (R2) Score
**Visualizations**
Feature importances of the best model are visualized using a horizontal bar chart.
A distribution plot compares actual vs. predicted ratings.
A scatter plot displays actual vs. predicted ratings.
A pair plot shows relationships between selected features and ratings.
Additional Visualizations
The script also includes additional visualizations, such as a distribution plot and scatter plot comparing actual vs. predicted ratings and a pair plot of selected features and ratings.
