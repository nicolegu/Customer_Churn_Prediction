# Bank Customer Churn Prediction
This project uses logistic regression, K nearest neighbors, and random forest models to predict customer churn. The dataset contains features and behavior of customers from a bank. The goal is to find the most important features that contribute to customer retention, and to propose business strategies accordingly.

In the context of banking, customer churn means customers close their accounts or discontinue using the services provided by a specific bank. High churn rates can be caused by issues such as lack of competitive products and poor customer experience. Therefore, monitoring customer churn and analyzing the driving forces behind the change in customer churn offer valuable insights into customer preferences, needs, and pain points.

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

## Suggestions
What types of customers do we want to attract?

The results from the logistic regression show that there is positive correlation between exit behavior and age, balance, and estimated salary. German or female customers are also more likely to exit. On the other hand, being an active member is negatively correlated with exit.