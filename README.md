# Final-Project
Predictive Maintenance and Anomaly Detection in Autonomous Vehicles Using Supervised and Unsupervised Machine Learning

This notebook performs a comprehensive analysis on a dataset of vehicle component data to classify failures and identify anomalies.

# How to Run the Code
Open in Google Colab: Click the "Open in Colab" button or upload the .ipynb file to your Google Drive and open it with Google Colab.
Run all cells: Go to the "Runtime" tab in the Colab menu and select "Run all". This will execute all the code cells sequentially.
Review the output: The notebook will display various outputs including tables, plots, and reports that summarize the results of the classification and anomaly detection tasks.
# Notebook Contents
The notebook covers the following key steps:

Setup and Data Loading: Installs necessary libraries, loads the dataset (simulated data using make_classification), and defines component names.
Data Preparation: Splits the data into training and testing sets for supervised learning.
# Supervised Learning (Classification):
Trains and evaluates three classification models: Random Forest, Gradient Boosting, and SVM.
Performs cross-validation and hyperparameter tuning using GridSearchCV and StratifiedKFold.
Presents a summary table of cross-validated and test set metrics for each model.
Visualizes the ROC curve and Confusion Matrix for the best performing classification model (Random Forest in this case).
Provides a classification report for the best model.
# Unsupervised Learning (Clustering & Anomaly Detection):
Applies KMeans and DBSCAN for clustering the data.
Uses Isolation Forest for anomaly detection.
Displays clustering metrics for KMeans.
Visualizes the data in 3D PCA projections colored by Failure, Anomaly, and KMeans Cluster.
Visualizes the data in 2D t-SNE projections colored by KMeans Cluster and Failure.
# Feature Analysis:
Shows the feature importance from the Random Forest model.
Displays a correlation heatmap between components and failure.
Calculates and visualizes the average component value difference between failure and no failure cases.
Anomaly Detection Evaluation: Provides precision, recall, and F1-score for the Isolation Forest anomaly detection.
Extra Visualizations: Includes a Parallel Coordinates plot and a table showing failure rate by KMeans cluster.
# Dependencies
The code requires the following libraries, which are automatically installed at the beginning of the notebook:

numpy
pandas
matplotlib
seaborn 
plotly
scikit-learn
# Note: The data used in this notebook is generated using make_classification for demonstration purposes. To use your own data, replace the "DATA PREPARATION" section with your data loading and preprocessing steps, ensuring your feature columns and target variable are correctly defined.
