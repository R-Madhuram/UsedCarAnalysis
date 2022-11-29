# UsedCarAnalysis

Used-cars trading business has been operational for many decades now. Price-assessment of used-vehicles is the premise of this trading business and this price reflects the objectives, fairness and nature of the used-vehicles markets. Hence, predicting the the price of used cars is of importance to used-car dealers that can be used to tune their inventory and selling price thereby increasing the profit margin. 
We were provided with a used-vehicle dataset with about 400K observations with 17 attributes and the price of each observations. Throughout the data-analysis and modeling we followed the CRISP-DM framework to conduct the data processing and evaluation. After conducting an initial exploratory data analysis of the dataset which included identification and removal of redundant features, identification and removal of outliers/erroneous data entry, encoding categorical variables, we performed multiple regression analysis to standardize and improve the accuracy of used-car price predictions. 
Our regression models included OLS (Ordinary least Squares Linear regression), Polynomial Bayesian ARD (Automatic Relevance Determination) and Polynomial Bayesian Ridge regression. We also used Grid Search to tune the hyper parameters of the model wherever it was computationally possible to improve the model accuracy. We combined permutation importance to find the features that were more deterministic of the price of the used-vehicles. We used Mean Absolute Error(MAE), Mean Absolute Percentage Error (MAPE), Mean Log Square Error (MLSE) and R^2 values as performance metric of the various models that were built. 
For the given data set we found that Polynomial Bayesian Ridge regression outperformed all other models with a MAE, MAPE, MLSE and R^2 value of (3886.3, 4958.3), (0.32 , 0.35), (0.15, 0.18) and (0.76,0.69) for the data set with and without removing unavailable data for the observations. Also, from the Pearson’s-correlation analysis and permutation importance of the model built we deduced that important features include, odometer reading, year, transmission, type(sedan, truck, bus etc), fuel (gas, hybrid, electric etc) and condition(new, fair, excellent etc.) in that order that affect the price of a used vehicle. The model proposed in this analysis has been able to bring down the baseline error metrics MAE, MAPE and MLSE by 60-70%,50% and 90% respectively with a fit of 0.7 or greater. Also the choice of Bayesian regression, which is a probabilistic model, gives us the ability to determine if an observation could be an outlier (eg: antique vehicle) along with its price prediction. This might aid in decision making while fine-tuning a used-car inventory and forecasting a sales price both of which can improve profitably of the business. This is particularly relevant to the dataset we analyzed that contained many outliers and vehicles that were 20 years or older (classic, antique and vintage cars).Classification approaches could probably improve the accuracy of the current model.  
We propose that future work that takes into consideration the complexity of the system (used car prices) like Grey relational analysis (GRA) filter along with regression like Back propagation Neural Net regression and more advanced hyper parameter tuning methods (like particle swarm optimization) might yield models with better accuracy for used car price prediction. Also, utilization of kernel tricks might  improve the performance of the model as well. Further, dataset with lesser data integrity issues could also be utilized to make predictions as used-car price prediction is well documented problem in machine-learning with many available datasets. 

Key-words: Used car price, Bayesian Ridge regression, permutation importance, Pearson’s-correlation

