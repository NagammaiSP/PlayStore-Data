Google Play Store Mobile App Dataset Analysis
Introduction
This repository contains an analysis of mobile applications available on the Google Play Store. The dataset provides valuable insights into various facets of these applications, enabling thorough analysis and prediction endeavors.

Dataset Columns
The dataset includes the following columns:

App: Name of the application.
Category: Category to which the application belongs (e.g., ‘Art & Design’, ‘Education’, ‘Finance’, etc.).
Rating: User rating of the application (ranging from 1 to 5 stars).
Reviews: Number of user reviews for the application.
Size: Size of the application (in kilobytes or megabytes).
Installs: Number of times the application has been installed from the Google Play Store.
Type: Whether the application is free or paid.
Price: Price of the application (if not free).
Content Rating: Content rating of the application (e.g., ‘Everyone’, ‘Teen’, ‘Mature 17+’, etc.).
Genres: Genre(s) to which the application belongs.
Last Updated: Date when the application was last updated on the Play Store.
Current Ver: Current version of the application.
Android Ver: Minimum required Android version for the application to run.
Data Preprocessing
The following preprocessing steps were applied to ensure clean data:

Size Conversion: The ‘Size’ column was converted to a consistent format (kilobytes or megabytes).
Installs Conversion: The ‘Installs’ column was converted to a numeric format.
Price Handling: Dollar signs were removed from the ‘Price’ column.
Missing Values: Rows with missing values in ‘Size’, ‘Installs’, ‘Price’, ‘Rating’, and ‘Reviews’ were dropped.
Feature Selection
We selected the following features for prediction:

‘Size’
‘Installs’
‘Price’
‘Rating’
‘Reviews’
The target variable is the ‘Category’ column, representing the app category.

Model Training and Evaluation
We trained five models using standardized features:

Decision Tree
Random Forest
Logistic Regression
Support Vector Machine (SVM)
K-Nearest Neighbors (KNN)
Evaluation metrics include precision, recall, F1-score, and accuracy. The Random Forest model performed best, achieving the highest accuracy and macro F1-score.

Visualization of Results
Confusion matrices and heatmaps were used to visualize true positive, false positive, true negative, and false negative predictions for each model.

Linear Regression
Additionally, we explored linear regression. The model’s R-squared score indicated that it explains only a fraction of the variance in the target variable. Mean squared error and mean absolute error highlighted significant deviations from actual values.
