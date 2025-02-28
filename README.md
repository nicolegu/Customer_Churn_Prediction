# Bank Customer Churn Prediction
This project uses logistic regression, K nearest neighbors, and random forest models to predict customer churn. The dataset contains features and behavior of customers from a bank. The goal is to find the most important features that contribute to customer retention, and to propose business strategies accordingly.

In the context of banking, customer churn means customers close their accounts or discontinue using the services provided by a specific bank. High churn rates can be caused by issues such as lack of competitive products and poor customer experience. Therefore, monitoring customer churn and analyzing the driving forces behind the change in customer churn offer banks valuable business insights into customer preferences, needs, and pain points.

## Project Structure
`data/': The dataset is from https://www.kaggle.com/code/kmalit/bank-customer-churn-prediction/data, containing features and exit behavior of 10,000 customers.

`images/': The folder contains data visualization and figures of model evaluation.

`Customer_Churn_Prediction.ipynb': The Jupyter notebook has codes for data exploration, feature preprocessing, model training and evaluation, and feature selection.

## Data Exploration
The dataset provides 10 useful attributes. 6 features are numerical, and 4 features are categorical. I use boxplots to show the distributions of numerical features for customers who exited and who stayed separately. The distributions of age, balance, and tenure are different across groups, suggesting these features can be important to explain why customers made different decisions. I use histograms to show the distributions of categorical features. Since there is significant difference in the distributions of country (market), gender, and whether the customer is an active member, these factors can also be vital to predict the decision of a customer.

![Boxplots of Numerical Features](images/feature_boxplot.png)
![Histograms of Categorical Features](images/feature_histogram.png)

## Model Training
I use 3 models to predict whether a customer stops doing the business with bank. The first model is logistic regression, and I use it as my benchmark model.

## Search for Optimal Hyperparameters
![Combinations of Regularization Methods and Regularization Rates](images/regularization_heatmap.png)


## Evaluation
![ROC curve of Logistic Classifier](images/roc_curve_LogisticReg.png)
![ROC curve of Random Forest](images/roc_curve_randomForest.png)
![ROC curve of K Nearest Neighbors](images/roc_curve_knn.png)

## Suggestions
What types of customers do we want to attract?

The results from the logistic regression show that there is positive correlation between exit behavior and age, balance, and estimated salary. German or female customers are also more likely to exit. On the other hand, being an active member is negatively correlated with exit.