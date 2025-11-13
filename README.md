# machine_learning_with_python

In this repository, we try to solve some projects in the field of machine learning methods such as regression, classification, and clustering, and ultimately arrive at good models that can predict new things. We use python and it's tools that run in Jupyter notebook. 

## Regression
We used the King County Housing Dataset from Kaggle that includes homes sold between May 2014 and May 2015, features 21 columns, and over 21,000 entries and it is saved in a cvs file in the data folder called kc_house_data.cvs.
The data has integer and float data types, some of which probably need to be changed. Also, at first glance, three columns are missing data, which need to be further examined and managed. 

For this project, we used the King County Housing dataset from Kaggle, which includes homes sold between May 2014 and May 2015, 21 columns, and over 21,000 entries. We intended to use the features of this dataset to estimate price in dollars, but in this experiment, we were not looking for the best formula for this purpose, but rather to show the way of thinking and the path to the model, as well as different regression methods, and also to test some of the features of Python in this context.
You can see our research on this topic in the file ML_With_python_Regression.ipynb.

## Classification
For each of the classification methods, we had considered different projects.
### K-Nearest Neighbors (KNN) Classification
We tried to do this project with walking through a full ML workflow with our selected dataset using KNN(K-Nearest Neighbors). We wanted to predict the primary hashtag category of an Instagram post based on engagement metrics and traffic sources. 
Our input included numeric engagement and traffic features per post and our output is predicted hashtag category (top 5 hashtags + “Other”).
The results help optimize posting strategy and predict content popularity by understanding what types of content users engage with.
For this project, we used Instagram Reach Analysis Data, includes 120 samples. Although the number of samples seems small, it is enough for our testing and learning for now.
Our workflow includes 7 steps, each of which is explained in detail in the file Predicting_Primary_Hashtag_Category_on_Instagram_Posts_Using_KNN.ipynb :
1. Problem Definition
2. Input Data (Features)
3. Preprocessing Steps
4. Train/Test Split
5. Model
6. Evaluation
7. Insights and Recommendations

We have improved the results in three stages with changes in data engineering, which are detailed in the file in question.

### Decision Tree Classification
We tried to predict whether a passenger in titanic survived using passenger attributes (class, age, sex, fare, family, embarkation, etc.). We downloaded from Kaggle train.csv file and uesd it and used a workflow like and we used the same workflow as in the previous part. 
The steps of this experiment, along with complete explanations and comments, are available in the Predicting_Passenger_Survival_Titanic_Using_Decision_Tree_Classification.ipynb file.

### Logistic Regression Classification
We tried to predict if a client will subscribe to a term deposit (target = y) based on demographic and campaign features. we used Features from Bank Marketing dataset (age, job, marital, education, default, balance, housing, loan, contact, day, month, duration, campaign, pdays, previous, poutcome)
Why Logistic Regression:
- Binary classification problem (yes/no).
- Interpretable coefficients, handles categorical/numeric features well.<br/>

The steps of this experiment, along with complete explanations and comments, are available in the Logistic_Regression_for_Customer_Conversion_Prediction_in_Bank_Marketing.ipynb file.

### SVM Classification
We tried to predict Wine Quality.
Project Overview: Wine Quality Classification (SVM)  the quality of red wine based on its physicochemical properties (e.g., acidity, sugar, pH, alcohol). we used the dataset winequality-red.csv comes from the UCI Machine Learning Repository. Each record represents a wine sample tested in a Portuguese wine lab, with 11 numeric input variables and one quality score (integer between 3 and 8).
Our goal was to build an SVM-based classification model that automatically categorizes each wine into one of three classes:
| Category | Description | Label |
| :- | :- | :- |
| Low | Quality ≤ 5 | 0 |
| Medium | Quality = 6 | 1 |
| High | Quality ≥ 7 | 2 |

why we used SVM in the Wine Quality Classification project:
- Handles nonlinear relationships – captures complex patterns with RBF kernel.
- Good for small/medium datasets – efficient with our wine data size (~1,500 samples).
- Robust to outliers – focuses on boundary samples (support vectors).
- Maximizes class separation margin – improves generalization and reduces overfitting.
- Effective with overlapping classes – suits wine data where class boundaries blur.
- Mathematically stable and well-founded – reliable optimization approach.
- Supports multiclass classification – easily extended with one-vs-rest (OvR).
- Strong baseline for tabular numeric features – fits structured physicochemical data well.
The steps of this experiment, along with complete explanations and comments, are available in the Wine_recognition_Using_SVM_Classification.ipynb file.


## clustering
- Clustering is an unsupervised machine learning technique that automatically groups data points into clusters (or segments) based on their similarity.
- It doesn’t use predefined labels — instead, it finds patterns or natural structures in the data.
- The goal is to make points within a cluster as similar as possible and points between clusters as different as possible.

### K-Means
- K-Means is a popular clustering algorithm that divides data into K distinct groups based on feature similarity.
- It works by:
    - Choosing K cluster centers (centroids) randomly.
    - Assigning each data point to the nearest centroid (based on distance, usually Euclidean).
    - Recalculating centroids as the average of all points in each cluster.
    - Repeating steps 2–3 until centroids stabilize (no significant change).
- The result: K-Means finds compact, well-separated clusters — for example, grouping mall customers into similar spending and income profiles.

Project "Customer Segmentation using K-Means Clustering" Overview: We try to Segment mall customers into distinct groups based on their behavior — mainly spending patterns, income, and age — to help the business understand customer types (e.g., low spenders, medium spenders, high spenders)

Why K-Means:
- Unsupervised learning method (no labels like “survived” or “yes/no”).
- Groups data based on similarity.
- Helps identify patterns and market segments automatically.
- Simple, efficient, and commonly used in marketing analytics.
Dataset: Mall_Customers.csv
CustomerID, Gender, Age, Annual Income (k$), Spending Score (1-100)

The steps of this experiment, along with complete explanations and comments, are available in the Mall_Customers_K_Means_Clustering.ipynb file.

### Hierarchical
Hierarchical clustering is a method that builds a hierarchy (tree structure) of clusters instead of assigning data points directly to a fixed number of groups.
It works by either merging small clusters step by step (agglomerative) or splitting large ones (divisive) until all data points form a hierarchy.
The result is shown as a dendrogram, a tree-like diagram that helps you decide how many clusters to choose visually.
Project Mall Customers – Hierarchical Clustering aims to use unsupervised machine learning — specifically Hierarchical Clustering — to automatically group customers based on their Annual Income and Spending Score.

Why Hierarchical Clustering :
- No need to predefine the number of clusters : Unlike K-Means, you don’t have to guess how many customer groups exist beforehand — the dendrogram visually shows the most natural number of clusters.

- Visual and interpretable structure : It builds a tree-like hierarchy (the dendrogram) that helps you see how customers merge or split at different levels — giving deeper insights into relationships among groups.

- Good for smaller to medium datasets : The Mall Customers dataset (~200 rows) is perfectly sized for Hierarchical Clustering, which can become slow with very large datasets.

- Captures nested relationships : It can reveal subgroups within clusters — for instance, “high spenders” can further split into “young professionals” and “older luxury buyers”.

- No randomness or initialization sensitivity : Unlike K-Means, which depends on random centroids and can yield different results per run, Hierarchical Clustering is deterministic and consistent.

Dataset: Mall_Customers.csv
CustomerID, Gender, Age, Annual Income (k$), Spending Score (1-100)
The steps of this experiment, along with complete explanations and comments, are available in the Mall_Customers_Hierarchical_Clustering.ipynb file.


## Services

If you like this project, I also offer professional **data cleaning and analysis services on Fiverr**:  
[Hire me on Fiverr](https://www.fiverr.com/hesamzia/clean-and-analyze-your-data)
