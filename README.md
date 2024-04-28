# weather-forecasting
Data Loading: The code starts by importing the pandas library and then reads a CSV file containing Seattle weather data into a DataFrame named df.

Data Exploration: The head() method is used to display the first few rows of the DataFrame to understand its structure and contents.
python

Handling Missing Values: The isna().sum() method is used to check for missing values in the DataFrame. This information is helpful for data preprocessing.

Data Preparation: The independent variables (features) are stored in the DataFrame X, which is created by dropping the 'date' and 'weather' columns from the original DataFrame df. The target variable is stored in the Series y, which contains the 'weather' column from the original DataFrame.

Splitting Data: The dataset is split into training and testing sets using the train_test_split function from scikit-learn. This allows the model to be trained on one portion of the data and evaluated on another portion.

Model Training: A logistic regression model is created using scikit-learn's LogisticRegression class, and it is fitted to the training data.

Model Evaluation: Predictions are made on the test set, and a classification report is printed to evaluate the performance of the model.

Prediction: A dictionary test_weather containing weather data for a specific instance is created. This data is then used to create a DataFrame test_df, which is passed to the trained model to make predictions.


This code snippet trains a logistic regression model to predict weather conditions in Seattle based on given features and evaluates its performance. Finally, it makes a prediction for a new instance of weather data.

Created By:- Yuvraj Sharma (225/UAI/013)
             Reeti Pandey (225/UAI/008)
             Unnati Pal (225/UAI/011)


