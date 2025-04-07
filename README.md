# Lab-1
MGT 665 - Lab 1

# Housing Prices Regression (India)

## Abstract
The goal of this project is to predict the prices of houses with similar characteristics (has a balcony, parking spaces, number of bathrooms, etc..). In order to accomplish this, Linear and Ridge regression were employed to help predict future house prices. Both methods were able to predict within 21,000 rupees which seems like alot; however, that equates to around $242 US dollars. 

## Introduction
We were provided with around 190,000 different properties from across India. Tasked with creating a model that would be able to predict the prices of houses that were about to come to the market.

## Related work
Eray Korkmaz ran a similar study with a different set of housing prices. He employed the same model I did as well as other models like a Random Forest Regressor and Decision Tree Regressor. In his study, linear regression was the worst method. I went into this study knowing that linear regression might not be the best method.

## Methodology
I started out this project by learning about the dataset. I quickly realized there were alot of categories that could have been numbers, but were a bunch of words instead. I quickly removed all the categories like the description, overlooking, and super area, as these columns did not provide much to the model. I then converted the amount column into the same demonination. In the original set, the denominations varied heavily, so converting to one denomination helped the machine understand easier. I then removed all the null values as they dont provide much either. As well as extracted the number of beds (BHK) before deleting the Title column. After all the preparation, I finally had a dataset that would be decent for linear regression.

## Results
LR MSE: 20,077.2660
RR MSE: 20,103.5390

The Linear regression model that I employed was slightly better than the ridge regression model. Both were able to predict the housing prices within about 20,000 rupees (around $200 USD).

## Discussion
The results came back suprisingly better than anticipated. I fully expected ridge regression to be alot more accurate than the linear regression; however, this wasnt the case. I do believe that with more fine tuning, the model can get alot more accurate as 20,000 rupees is still alot in India, even though it only is equivalent to about $200 USD. 

## References
Korkmaz, E. (2025, March 25). Housing Price Prediction Machine Learning. Kaggle. https://www.kaggle.com/code/eraykorkmaz/house-price-prediction-machine-learning 
