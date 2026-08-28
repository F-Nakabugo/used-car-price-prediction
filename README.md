## Predicting the Selling Prices of Used Cars: A Comparison of Three Regression Models
### Introduction
The project is an end-to-end Machnine Learning task using a small dataset containing the history of used cars to build and compare three regression models to predict selling prices of the cars. 
### Objectives
- To build a Multi Linear Regression, Decision Tree, and Random Forest models. 
- To compare the algorithms and report their performance
### Key Results 
Overall, the most popular car brands also had relatively lower selling prices. 
Random forest was the best model evaluated. 
The prediction errors were still substantially large. This could be associated with the presence of duplicate records and the limited number of car characteristics in the dataset. 
### Dataset 
The data used was obtained from Kaggle. It contained information about used vehicles from online listings with 8128 records, with 4 predictor variables (`brand, km_driven, fuel, owner`) and `selling_price` as the target.  
The dataset did not have any misssing values. It however, had 1678 duplicate rows accounting for about 21% of the entire dataset.   
Here is the [link](https://www.kaggle.com/datasets/ahmedfakhar123/used-car-price-prediction-dataset/data?select=Used_Car_Prices.csv)
### Exploratory Data Analysis
The most popular car brands were Maruti, followed by Hyundai, and Mahindra. Most cars in the dataset were first-owner vehicles. Luxurious car brands like Mercedes-Benz, BMW, and Volvo had relatively large price ranges as compared to the less luxurious brands. 
### Methodology
The categorical features were transformed using One-Hot encoding while the `km_driven` feature was standardized.  
The datased was split into 80% training set and 20% testing set.   
Three models i.e., Multilinear Regression, Decision Tree, and Random Forest were trained and evaluated using R², MAE, and RMSE.    
A prediction error analysis evaluation of the best model was performed. 
### Models and Evaluation 
Evaluation was done using 3 metrics, and here is the summary of results:   
| Model | R² | MAE | RMSE |  
|---|---:|---:|---:|
| Linear Regression | 0.778 | ₹216,466 | ₹381,605 |
| Decision Tree | 0.783 | ₹184,174 | ₹377,504 |
| Random Forest | 0.824 | ₹177,752| ₹340,132 |  
### Limitations 
The model used only 4 predictor variables which made it harder to clearly distinguish between vehicles leading to a higher value of duplicate records. 
### Technologies used
- Scikit learn
- Pandas
- Matplotlib
- Seaborn



















