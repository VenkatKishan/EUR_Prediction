# EUR_Prediction
Predict Estimated Ultimate Recovery for Multistage Hydraulically Fractured Wells in Shale Formation

Background

The economic feasibility and production improvement of an oil and gas well largely depend on the efficiency of hydraulically generated fractures. Reserve estimation is the key step for economic and investment calculations. Reserve, estimated ultimate recovery (EUR), is the estimation of oil and gas volume that can be economically extracted under the current technological constrictions. Estimating EUR in very tight reservoirs and shale plays has long been challenging. Reserve assessment is a process that regularly updated the age of the reservoir production history. The data availability and the forecasting method are the two vital elements that determine the estimated EUR accuracy. Therefore, the development strategies are highly dependent on the accuracy of the forecast. The high-confidence EUR estimate is the total hydrocarbon recovery when the well reaches the abandonment conditions.

Therefore This Study proposes the use of different machine learning techniques to predict the EUR from a data set of 200 well production data and completion designs was collected from oil production wells in the Niobrara shale formation.The ML model to predict the EUR from the completion design parameters at an early time without the need for complex numerical simulation analysis. The developed models require only the initial flow rate(IP) along with the completion design(another set of features) to predict EUR with high certainty without the need for several months of production similar to the DCA models.

Goal Of The Project

We start by loading the  data, identify and address possible missing data, address outliers, 
create new features, and impute missing values using KNN. 
#1: Develop a voting-based ensemble of four data-driven models to predict Initial 
Production. 
#2: Develop a voting-based ensemble of four data-driven models to predict Estimated 
Probable  Recovery  (EUR).  Save  the  best model  and  deploy the  best model  on the  hold  out  data 
to predict EUR.
We Used 'ElasticNet','KNN','SVR','RandomForest','GradientBoosting' are our ML models and select best out of them by comparing each of model's RMSE and MAE score.

Result
We got GradientBoosting as the best model after deploying it on training and test dataset with a RMSE score of 2.983973e+06 which is still lot better compared to high production volume and time tradeoff!!!. 

Refrences

https://www.hindawi.com/journals/cin/2022/7084514/
https://onepetro.org/EM/article-abstract/8/01/23/205905/Machine-Learning-as-a-Reliable-Technology-for
https://www.mdpi.com/1996-1073/14/12/3629
https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.VotingRegressor.html
