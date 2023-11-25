# Bike-Sharing-Demand

Step 1: Imported necessary Libraries, Data Loading and Exploration
* Loaded the bike-sharing dataset from a CSV file into a Pandas DataFrame.
* Displayed the shape of the dataset, the first few rows, information about data types and non-null counts, null values count, and summary statistics.

Step 2: Data Visualization
* Created a histogram to visualize the distribution of the 'count' variable.
* Generated scatter plots to explore the relationship between temperature ('temp') and bike count.
* Used box plots and bar plots to understand the impact of season, holiday, and working day on bike counts.

Step 3: Time Series Analysis
* Converted the 'datetime' column to datetime data type.
* Plotted a time series line chart for 'datetime' vs 'count'.
* Extracted features like hour, grouped by hour, and visualized the average count for each hour.
* Extracted features like month, grouped by month, and visualized the total count for each month.

Step 4: Categorical Data Analysis
* Created a bar plot to compare bike counts on working days and non-working days.

Step 5: Feature Engineering
* Extracted features such as hour, day, month, and year from the 'datetime' column.
* Created dummy variables for categorical columns ('season', 'holiday', 'workingday', 'weather') using one-hot encoding.
* Dropped unnecessary columns like 'datetime', 'casual', and 'registered'.
* Applied the natural logarithm transformation (log1p) to the 'count' variable.

Step 6: Model Training and Validation
* Split the dataset into training and testing sets (70-30 ratio).
* Installed the XGBoost library.
* Imported XGBoost and GridSearchCV for hyperparameter tuning.
* Defined a parameter grid for tuning XGBoost hyperparameters.
* Conducted a grid search with cross-validation to find the best hyperparameters.
* Trained the final XGBoost model with the best parameters.

Step 7: Model Evaluation
* Predicted bike counts on the test set and evaluated the model performance.
* Calculated metrics such as mean squared error, mean absolute error, and R-squared.
* Visualized prediction errors using a histogram.

Step 8: Cross-Validation
* Conducted k-fold cross-validation (k=10) to assess the model's robustness.
* Calculated the mean and standard deviation of R-squared scores.
