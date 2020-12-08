# Used car price prediction using diffrent regression models.
In this small project I used the used car [dataset](https://www.kaggle.com/nehalbirla/vehicle-dataset-from-cardekho/notebooks) from Kaggle to predict 
selling prices of used cars.

# Things Learnt
* Dealing with incomplete data
* Data Cleaning
* Data visualization
* Stratified sampling
* Hyperparameter Tuning
* Different regression models

# Insights gained
From my intial handling of the dataset I found out that there were many missing values that had to either be removed or
filled in. The dataset then had to be split using stratified sampling due to the wide range of cars and selling prices. The correlation between the
selling price and the max power of the car was very strong and from this I gave 2 more attributes to the dataset as it may help with better predictions
those were **bhp/cc** and **bhp/seat**. 

Then the dataset was passed through 3 Regrssion models which were:
* Linear Regressor
* Decision Tree Regressor 
* Random Forest Regressor

The Mean and STD for each are as follows:
* Linear Regressor : *Mean 200428.7627*, *Standard Deviation: 51512.9411*
* Decision Tree Regressor: *Mean 212996.7645*, *Standard Deviation: 68163.2524*
* Random Forest Regressor: *Mean 172750.1854*, *Standard Deviation: 53068.7194*

From this we can see that the Random Forest Regressor faired a little bit better from the other two models. 
We can see that these predictions are okay but not that great. This can most probably improved by better handling of the missing data
or by gaining more data as this dataset conisted of roughly 8000 non-null rows.

# Conclusion
This model is nowhere close for deployment in the real world but a bit more tuning the dataset and 
getting more data will go a long way in making this model more accurate.

