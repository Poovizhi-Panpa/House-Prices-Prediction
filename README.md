# House-Prices-Prediction
This project predicts house sale prices using the Ames Housing dataset. It applies feature preprocessing, regression models, and hyperparameter tuning to build a robust prediction pipeline.

## Workflow

1. Data Preparation
- Handled missing values (domain-driven fills for categorical, median for numerical).
- Converted MSSubClass to categorical.
- Scaled numerical features with StandardScaler.
- Encoded categorical features with OneHotEncoder.

2. Modeling
- Baseline model: Linear Regression (numerical only).
- Regularized models: Ridge & Lasso Regression.
- Ensemble model: Random Forest Regressor.
- Hyperparameter tuning with cross validation: GridSearchCV.

3. Evaluation Metrics
- R² Score
- Mean Squared Error (MSE)

## Results

|Model	              |R² Score      |Notes|
|------|----|-----|
|Linear Regression	  |0.826        	|Baseline (numerical only)|
|Ridge Regression	    |0.878	        |Better with multicollinearity|
|Lasso Regression	    |0.895	        |Strongest linear model|
|Random Forest	      |0.892	        |As good as Lasso|
|Grid Search CV      |0.899          |Lasso is still the strongest model|
