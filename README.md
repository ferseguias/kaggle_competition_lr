# project_3_kaggle_competition_lr
![portada](https://raw.githubusercontent.com/Ironhack-Part-Time-Enero2022/Kaggle_competition/master/images/PORTADA.jpg)

To visit Kaggle competition and see results, click [here](https://www.kaggle.com/competitions/diamonds-part-datamad0122).

# Objetive 🎯
Apart from the obvious objective of winning the competition, I focused efforts on understanding data through exploration and online research of the topic. Also, applied data cleaning techniques, outliers management, encoding and standarization prior to testing linear regression models to get best predictive stats.

# Models tested 🤖
- DecisionTreeRegressor `from sklearn.tree import DecisionTreeRegressor`
- RandomForestRegressor `from sklearn.ensemble import RandomForestRegressor`
- GradientBoostingRegressor `from sklearn.ensemble import GradientBoostingRegressor`
- XGBoost `import xgboost as xgb`

# Step by step of the process 🏃🏽‍♂️
1. Problem understanding: data exploration with visualization and online research to get fundamental knowleadge of the field we are analizyng in order to improve our decisions and results. Detect correlations between variables and plot analyzed data.

![portada](https://raw.githubusercontent.com/ferseguias/project_3/main/images/Screenshot%202022-05-26%20at%2021.56.01.png)

2. Prepare data for applying models: remove inconsistent data, outliers management and provide data strucure, encoding and standarizarion of X variables prior next step.

3. Machine learning: once the data is clean and variables are carefully selected, trial and test is key. It is important to be able to evaluate our model, this is why `train`, `test` split has to be used `from sklearn.model_selection import train_test_split`. 80% of data is used to train the model, remaining 20% to evaluate it's performance. Big differences between stats on predicted train and test might evidence under/over fitting. Our goal is to get the lower RMSE (standard deviation of the residuals - prediction errors). A nice way to get the best combination of parameters for each model is using GridSearchCV tool `from sklearn.model_selection import GridSearchCV`. A set of parameters are provided and the model is evaluating each combination to get best parameter set.

4. Compare results: after several trials, many outcomes should be analyzed in order to find the most effective predictive model to be applied to `test.csv` provided by competition organizer.

5. Predict and submit results: before running the predictive model into test data, all transformation procedures applied to the data used for training should be applied accordingly to test. It is suggested to re-train the model using 100% of train data (without splitting 80%-20%) to get adjusted results in prediction.

# Results 📈
According to the best model submitted during the competition, my prediction has RMSE of 0.09494 which represents a 2.34% error over real price (price range = 4.055).

# Tools 🔧

[pandas](https://pandas.pydata.org/)

[matplotlib](https://matplotlib.org/)

[scikit-learn](https://scikit-learn.org/stable/)
