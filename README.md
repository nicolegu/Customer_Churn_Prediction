# Bank Customer Churn Prediction
This project uses logistic regression, K nearest neighbors, and random forest models to predict customer churn. The dataset contains features and behavior of customers from a bank. The goal is to find the most important features that contribute to customer retention, and to propose business strategies accordingly.

## Project Structure
`data/': a dataset containing customer features and exit behavior
`images/': data visualization and evaluation figures

## Data Visualization
![Boxplots of Numerical Features](images/feature_boxplot.png)
![Histograms of Categorical Features](images/feature_histogram.png)

## Search for Optimal Hyperparameters
![Combinations of Regularization Methods and Regularization Rates](images/regularization_heatmap.png)


## Evaluation
![ROC curve of Logistic Classifier](images/roc_curve_LogisticReg.png)
![ROC curve of Random Forest](images/roc_curve_randomForest.png)
![ROC curve of K Nearest Neighbors](images/roc_curve_knn.png)