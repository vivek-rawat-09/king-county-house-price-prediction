# King County House Price Prediction

## About the Project

This project was created to apply the machine learning concepts I learned during my machine learning course.

The goal is to predict house prices using the King County housing dataset while practising the complete machine learning workflow, including data exploration, preprocessing, feature engineering, model training, evaluation and hyperparameter tuning.

## Dataset

The King County housing dataset contains information about house sales along with different property characteristics such as:

- Bedrooms and bathrooms
- Living area and lot size
- Number of floors
- Waterfront and view
- Condition and grade
- Year built and renovated
- Latitude and longitude
- Zipcode
- House price

The target variable for this project is `price`.

## Exploratory Data Analysis

Before training the models, I explored the dataset to better understand the features and their relationship with house prices.

This included:

- Checking the dataset structure and missing values
- Analysing feature distributions
- Looking at correlations with house price
- Identifying skewed features and outliers
- Visualising geographical patterns using latitude and longitude

## Data Preprocessing & Feature Engineering

I performed preprocessing and created additional features from the existing data.

Some of the engineered features include:

- House age
- Sale year and month
- Renovation status
- Basement availability
- Living area per bedroom
- Bathrooms per bedroom
- Living area to lot-size ratio
- Geographical distance features

I also experimented with log transformations for skewed features and the target variable.

In the later stages of the project, I used scikit-learn pipelines and custom transformers to combine feature engineering, preprocessing and model training into a reusable workflow.

## Models Tested

I experimented with multiple regression algorithms:

- Linear Regression
- Random Forest Regressor
- Gradient Boosting Regressor
- Histogram Gradient Boosting Regressor
- XGBoost
- LightGBM

The goal was to compare different approaches and understand how different regression algorithms behave on the same dataset.

## Model Evaluation

The models were evaluated using regression metrics such as:

- Mean Absolute Error (MAE)
- Root Mean Squared Log Error (RMSLE)
- R² Score

Cross-validation was also used to obtain a more reliable comparison between models instead of relying only on a single train/test split.

## Hyperparameter Tuning

After comparing the models, I experimented with hyperparameter tuning to improve their performance.

I used:

- `GridSearchCV`
- `RandomizedSearchCV`

This allowed me to test different parameter combinations and select better configurations for the models.

## Final Result

After comparing and tuning the different regression models, **LightGBM** achieved the best performance among the models tested.

- **Test MAE:** 0.1157684159876091
- **Test R²:** 0.9032966986957912

## Machine Learning Pipeline

I also experimented with scikit-learn tools such as:

- `Pipeline`
- `ColumnTransformer`
- Custom transformers
- `TransformedTargetRegressor`

These helped organise the preprocessing, feature engineering and modelling steps into a consistent workflow.

## Tools & Libraries

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- scikit-learn
- XGBoost
- LightGBM
- JupyterLab

## What I Learned

This project helped me put the concepts from my machine learning course into practice and better understand how the different stages of a machine learning project connect together.

Some of the main concepts I practised were:

- Exploratory data analysis
- Data preprocessing
- Feature engineering
- Handling skewed data
- Train/test splitting
- Regression algorithms
- Model evaluation
- Cross-validation
- Hyperparameter tuning
- Machine learning pipelines
- Avoiding data leakage

This project was mainly created as a practical learning exercise to strengthen my understanding of machine learning with Python and scikit-learn.