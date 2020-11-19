# M5-Forecasting
M5 Forecasting

This project is to model the sales of the next 28 days for more than 30,000 products for Walmart.

M5 Forecasting is a well know competition in kaggle realized every year and it is separated in two. The first is to forecast the demand of each product. The second is to predict the mean and some percentiles. We will focus only in the first.\
        M5 Forecasting - Accuracy: https://www.kaggle.com/c/m5-forecasting-accuracy \
        M5 Forecasting - Uncertainty: https://www.kaggle.com/c/m5-forecasting-uncertainty
        
More information on: https://mofc.unic.ac.cy/m5-competition/

In this Github there are four codes.

"M5 Forecasting - Accuracy - Data study" is several analysis of the data consistency, and studies like the autocorrelation and partial autocorrelation; 

"M5 Forecasting - Accuracy  - Variables" contains the construction of new variables;

"M5 Forecasting - Accuracy  - Model" contains the ARIMA model used to forecast of the next 28 days; and

"holdout", this file is important because it contains not only the holdout but some final studies and considerations of our model.


One interesting thing about this project is that we decided to model one ARIMA per product. Therefore, the most challenging part was how to automate the parameter and the varaible selection. Moreover, the data size that exceded 16GB, this was a problem not only because we used computers with 16 GB and 12 GB of memory, but also because any code that we run was extremely time consuming. To deal with the memory problem, we decided to create one database per product; and to deal with the time problem, we decided to run several jupyter notebooks at the same time using Google Colaboratory. 
