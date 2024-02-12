# Airbnb-price-prediction
The dataset contains information about Airbnb in New York. Price analysis can reveal a lot. Show the dependence of prices on the area and on the area of ​​the apartment. Nowadays, Airbnb performs an indispensable function for both tourists and ordinary citizens, so housing prices should be objective, that is, reflect the quality of the map/house, as well as its location.Automating prices can be a challenge for a company like Airbnb. After all, housing prices are always changing and you need to adapt to the changes. For this purpose, a prediction model is built that can predict prices for new houses/apartments.

## Content
- [technologies](#technologies)
- [EDA](#EDA)
- [Prediction](#Prediction)

## Technologies
- Pandas - for loading data
- Matplotlib - for visualization 
- Seaborn - for visualization
- Sklearn - for preprocessing and modeling
- Xgboost - for modeling 
- Catboost - for modeling 
- Optuna - for tuning 


## EDA
Average Monthly Sales

![image](https://github.com/Anton4wave/Walmart-forecasting/assets/100091790/b3e07597-b6ad-42e6-aa82-3722af47bfa7)

Average Year Sales

![image](https://github.com/Anton4wave/Walmart-forecasting/assets/100091790/cf226b81-bad3-437f-97a3-9e1ff4106045)

The impact of holidays on sales

![image](https://github.com/Anton4wave/Walmart-forecasting/assets/100091790/64aa7e79-98ce-4ea6-bcc1-f50ba5bacb49)

Effect of Temperature

![image](https://github.com/Anton4wave/Walmart-forecasting/assets/100091790/e9dc97fc-722e-4ce3-b41f-f236c570f2c1)


A couple of conclusions can be drawn:

-Firstly, the number of sales depends greatly on the month

-Secondly, Walmart's sales are falling every year

-Thirdly, according to statistics, there are more sales during the weekend


## Prediction 

Metrics for this competition: The metric of the competition is weighted mean absolute error (WMAE). Weight of the error changes when it is holiday.

![image](https://github.com/Anton4wave/Walmart-forecasting/assets/100091790/174b5c63-27ee-45c3-bf17-e1a97a9a40d0)

Modeling:
-For the baseline I used RandomForestRegressor and get WMAE = 

-Then I removed unnecessary columns and trained the model again, obtaining WMAE = 

-Then I used XGBoost and got the best value. WMAE = 

