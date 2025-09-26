# House Prices Advanced Regression Techniques - EDA & Modeling

This project is part of the "21 Days 21 Projects" challenge and focuses on predicting house prices using the Kaggle "House Prices: Advanced Regression Techniques" dataset. The workflow includes data loading, cleaning, feature engineering, exploratory data analysis (EDA), model building, and hyperparameter tuning.

## Project Structure

- `day3houseprice.ipynb`: Main Jupyter notebook with all code and analysis.
- `submission.csv`: Output file for Kaggle submission.

## Steps Performed

1. **Data Loading**
   - Downloaded the dataset using Kaggle API.
   - Loaded train and test data with pandas.

2. **Exploratory Data Analysis (EDA)**
   - Visualized the distribution of `SalePrice` and its log transformation.
   - Analyzed feature correlations using heatmaps.

3. **Data Cleaning & Feature Engineering**
   - Imputed missing values for both numerical and categorical features.
   - Created new features such as `TotalSF`, `TotalBath`, and `Age`.
   - Applied one-hot encoding to categorical variables.

4. **Modeling**
   - Split data into training and validation sets.
   - Scaled features for linear models.
   - Trained Linear Regression and XGBoost models.
   - Evaluated models using RMSE, MAE, and R².

5. **Prediction & Submission**
   - Made predictions on the test set using the best model (XGBoost).
   - Reversed log transformation for final predictions.
   - Saved results to `submission.csv`.

---
