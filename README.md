# SC1015 Mini Project : Diamond Price Prediction

<p align="center">
  <img src="Dataset/diamonds.jpg" alt="Diamond Picture" width="800"/>
</p>


## About This project ##
This is a Mini-Project for the SC1015 (Introduction to Data Science and Artificial Intelligence) offered by the Nanyang Technological University, Singapore  during the AY22/23 Semester 2.
 
We will be focusing on an diamond price predictor in this project.

Here is the walkthrough of our project.



## Predicting Price of Diamonds for Public Looking to Buy Diamonds ## 
In general, people have limited knowledge about the prices of diamonds and diamond sellers capitalise on this by selling diamonds with unfair and unreasonable prices. 
Therefore, we are going to design and implement a prediction model for people to predict the prices of diamonds based on the **4Cs (Colour, Clarity , Cut , Carat)** . With that, people can have a better understanding on the prices of diamonds depends on the quality of 4Cs and they can have a reliable indicator or estimation on the diamond prices before purchasing to ensure they have purchased the diamonds at a fair price.


## The available features are: ##


PRICE : Diamond price in USD

CARAT : Weight of the diamond (1 carat equals 0.2 grams).

CUT : Quality of the cut (Ideal, Premium, Very Good, Good, Fair).

COLOR : Diamond colour, from D (Best) to J (Worst).

CLARITY : Measurement of how clear the diamond is (IF (Best), VVS1, VVS2, VS1, VS2, SI1, SI2, I1 (Worst)).

DEPTH% : Measure of the depth in relation to the width of the diamond’s table, calculated as --> Depth (%) = Depth (mm) / Diameter (mm)

TABLE : Top facet of the stone; table percentage is the ratio between the table size and the diameter of the diamond

X : Length in mm

Y : Width in mm

Z : Depth in mm
 
## Models Used ##
1. Linear Regression
2. Random Forest Regression (3 versions) with hyperparameter tuning
3. XGBoost Regressions (3 versions) with hyperparameter tuning

## Conclusion ##
In conclusion, we have faced different limitations thorughout the preparation of this project. The large dataset used in this project is difficult to observe in detail. Hence, with the proper use of different graphs and plots, the details can be clearly understood such as the spread of data, trend of data and relationship between the variables. Beside, the dataset contains a lot of categorical data, which limits the implementation of regression in the training process. By implementing label encoding, the categorical data is converted to numerical data, which can be used in the regression model as well. 

Based on different performace metrics(RMSE and R^2) to predict the accuracy of our models, we found out that Random Forest Regression (V3) is the most accurate model which can predict the price of diamond. 

The customers who are purchasing diamonds will be able to use the UI developed based on our best machine learning model to predict the price of diamonds they are going to purchase and determine if the price set by the diamond sellers are similar to the price predicted. 

Thus, we can avoid customers overpaying for diamonds. With that, we believe that our project has somewhat developed a solution which can be used in partical terms.

For the future improvement, exploration of more hyperparameters in the regression model is importatnt to further optimize the training model performance. More predictors such as the dimension of diamond should be included in the training process if the information about the predictors are more readily accessible to the customer in the future. In reality, the dataset might be too clean with very little outliers and null values which might have made our machine learning prcocesses slightly easier. 

## What did we learn? ##
- How to use github to collaborate with other peers in a team project
- Solve real world problems using proper real world related dataset
- Perform regression model which is not covered in class (XGBoost)
- Proper tuning of hyperparameter to avoid overfitting or underfitting
- Program a User Interface (UI) to easily estimate the diamond price
## Contributors ##
| Name              |                    Contributions                     |
|---|:---:|
|Selvakumar Karthik Adharsh | Label Encoding,Linear and Random Forest Regression, Presentation Slides, Video Presentation |
| Beh Jia Jiunn | Data Preparation, Exploratory Data Analysis, Presentation Slides, Video Presentation, |      
|  Tan Wu Ji |   XGBOOST Regression, Prediction UI, Presentation Slides, Video Presentation |

## References ##
1. https://www.geeksforgeeks.org/xgboost/?ref=rp
2. https://shira-diamonds.com/about/education/4-cs/
3. https://4cs.gia.edu/en-us/diamond-color/
4. https://www.onlinediamondbuyingadvice.com/diamond-education/diamond-clarity/
5. https://bnsec.bluenile.com/bnsecure/certs/LD13571559/GIA?country=USA&language=en-us
6. https://www.globenewswire.com/news-release/2014/12/09/689825/10111532/en/NEW-STUDY-Americans-Overpaying-by-as-Much-as-72-for-an-Engagement-Ring.html
7.https://scikitlearn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html#:~:text=A%20random%20forest%20regressor.,accuracy%20and%20control%20over%2Dfitting.

