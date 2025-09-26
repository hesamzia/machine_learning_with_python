# machine_learning_with_python

In this repository, we try to solve some projects in the field of machine learning methods such as regression, classification, and clustering, and ultimately arrive at good models that can predict new things. We use python and it's tools that run in Jupyter notebook. 

## Regression
We used the King County Housing Dataset from Kaggle that includes homes sold between May 2014 and May 2015, features 21 columns, and over 21,000 entries and it is saved in a cvs file in the data folder called kc_house_data.cvs.
The data has integer and float data types, some of which probably need to be changed. Also, at first glance, three columns are missing data, which need to be further examined and managed. 

For this project, we used the King County Housing dataset from Kaggle, which includes homes sold between May 2014 and May 2015, 21 columns, and over 21,000 entries. We intended to use the features of this dataset to estimate price in dollars, but in this experiment, we were not looking for the best formula for this purpose, but rather to show the way of thinking and the path to the model, as well as different regression methods, and also to test some of the features of Python in this context.
You can see our research on this topic in the file ML_With_python_Regression.ipynb.

## Classification
For each of the classification methods, we had considered different projects.
### K-Nearest Neighbors (KNN) 
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

## clustering