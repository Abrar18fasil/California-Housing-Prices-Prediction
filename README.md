# California-Housing-Prices-Prediction
##Overview

This project involves predicting housing prices in California using data from the California Housing Dataset. The dataset includes various features such as median income, house age, and location, which influence housing prices. The goal is to build a regression model that accurately predicts the target variable: median house value.

Dataset

Source: Kaggle - California Housing Prices Dataset 
link 🔗  :https://www.kaggle.com/datasets/camnugent/california-housing-prices

##Features:

longitude: Longitude of the property.

latitude: Latitude of the property.

housing_median_age: Median age of houses in the area.

total_rooms: Total number of rooms in all houses in the area.

total_bedrooms: Total number of bedrooms in all houses in the area.

population: Total population of the area.

households: Total number of households in the area.

median_income: Median income of households in the area.

ocean_proximity: Proximity to the ocean (categorical feature).

median_house_value: Median house value (target variable).

##Installation

Clone the repository:

git clone <repository-url>

Install the required dependencies:

pip install -r requirements.txt

Download the dataset from Kaggle and place it in the data/ directory.

Preprocessing Steps

##Loading the Data:

The dataset is loaded into a pandas DataFrame.

##Handling Missing Values:

Missing values in total_bedrooms are imputed using the median strategy.

##Encoding Categorical Features:

The ocean_proximity feature is encoded using one-hot encoding.

##Feature Scaling:

Numerical features are scaled using StandardScaler to normalize the data.

##Model Training

We use a Linear Regression model as the baseline to predict house prices.

Steps:

Split the data into training and testing sets (80% train, 20% test).

Train the Linear Regression model on the training data.

Evaluate the model on the test set using the following metrics:

Mean Absolute Error (MAE): Measures the average absolute difference between predicted and actual values.

Root Mean Squared Error (RMSE): Penalizes larger errors more heavily, indicating overall model accuracy.

R-squared (R²): Proportion of the variance in the target variable explained by the model.

##Results:

Mean Absolute Error (MAE): 50,670.74

Root Mean Squared Error (RMSE): 70,060.52

R-squared (R²): 0.625

##Visualization

The dataset was visualized to explore correlations and understand feature relationships:

Heatmap of feature correlations.

Scatter plots to analyze relationships between median_income, house_age, and median_house_value.


##Conclusion

The Linear Regression model provides a good baseline with an R² of 0.625, explaining 62.5% of the variance in housing prices. However, there is room for improvement by trying advanced models like Random Forest or Gradient Boosting.
