# machine_learning_with_python

In this repository, we try to solve some projects in the field of machine learning methods such as regression, classification, and clustering, and ultimately arrive at good models that can predict new things. We use python and it's tools that run in Jupyter notebook. 

## Regression
For this project, we have collected data on approximately 4000 apartments in a city. All data is completely real. We want to estimate the price in dollars using the features of this dataset. The data is stored in the file housePrice.csv.
The building specifications include the following:
- Area of ​​the house in meters (Area)
- Number of bedrooms (Room)
- Parking or not (Parking)
- Warehouse or not (Warehouse)
- Elevator or not (Elevator)
- Address of the area (Address)
- Price in dollars (Price(USD))
In this dataset, some houses do not have addresses and the area of ​​some houses is entered incorrectly (they have very large values). For this purpose, we also need to manage these items and remove them from our dataset.
### Simple Linear Regression
In the first step, we tried to build a model with simple linear regression. We first tried the area column and then the room. The evidences show that we cannot find a good model to predict apartment prices with simple linear regression through a single column.
### Multiple Linear Regression
In the second try we use Multiple Linear Regression in three test. First with 2 column (Area and Address), second 3 column(Area, Address and Room) and third all column (Area, Address, Room, Parking, Elevator and Warehouse).
All tests are unsuccessful and results are about 55%. This shows that Multiple Linear Regression is not as successful as Simple Linear Regression.

## Classification

## clustering