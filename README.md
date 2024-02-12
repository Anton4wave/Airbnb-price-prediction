# Airbnb-price-prediction
The dataset contains information about Airbnb in New York. Price analysis can reveal a lot. Show the dependence of prices on the area and on the area of ​​the apartment. Nowadays, Airbnb performs an indispensable function for both tourists and ordinary citizens, so housing prices should be objective, that is, reflect the quality of the map/house, as well as its location.Automating prices can be a challenge for a company like Airbnb. After all, housing prices are always changing and you need to adapt to the changes. For this purpose, a prediction model is built that can predict prices for new houses/apartments.

## Content
- [Technologies](#Technologies)
- [EDA](#EDA)
- [Prediction](#Prediction)
- [Conclusion](#Conclusion)

## Technologies
- Pandas - for loading data
- Matplotlib - for visualization 
- Seaborn - for visualization
- Sklearn - for preprocessing and modeling
- Xgboost - for modeling 
- Catboost - for modeling 
- Optuna - for tuning 


## EDA
Scatterplot of neighbourhood

![image](https://github.com/Anton4wave/Airbnb-price-prediction/assets/100091790/092a114f-1b37-46be-8b14-023a2ca8c480)

Histograma of Room type 

![image](https://github.com/Anton4wave/Airbnb-price-prediction/assets/100091790/3b5a95a5-3d12-477b-8e25-dc09a102a2b2)

Histograma of neighbourhoods

![image](https://github.com/Anton4wave/Airbnb-price-prediction/assets/100091790/640d218a-847c-4b44-ab32-6f25878df895)


## Prediction 

Metrics for this project: For this task, I took RMSE as a metric

Modeling:

- As Baseline I took XGBRegressor and RandomForestRegressor with Kfold 

- Then tuning with Optuna for CatboostRegressor

- Final model with CatboostRegressor with best parameters

- Got RMSE = 79 - best value 

![image](https://github.com/Anton4wave/Airbnb-price-prediction/assets/100091790/fb04095b-3d17-45a1-ae4e-ea9692010658)


## Conclusion 

Trained a model with RMSE = 79 and received feauture importance of CatBoost. It can be argued that the most important feature influencing the price is Entire home and minimum nights. Prices depending on the area can be seen in this graph:

![image](https://github.com/Anton4wave/Airbnb-price-prediction/assets/100091790/640ded07-7731-47a3-93f9-2ca5400d880f)

