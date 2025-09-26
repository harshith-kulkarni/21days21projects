# Heart Disease Prediction - EDA & Machine Learning

This project is part of the "21 Days 21 Projects" challenge and focuses on predicting heart disease using the UCI Heart Disease dataset. The workflow includes data loading, cleaning, exploratory data analysis (EDA), feature engineering, model building, evaluation, and model saving.

## Project Structure

- `day4heartdiseaseprediction.ipynb`: Main Jupyter notebook with all code and analysis.
- `best_heart_disease_model.joblib`: Saved best model for deployment or inference.

## Steps Performed

1. **Data Loading**
   - Downloaded the dataset using KaggleHub.
   - Loaded the CSV data into a pandas DataFrame.

2. **Exploratory Data Analysis (EDA)**
   - Inspected data structure, types, and missing values.
   - Visualized target distribution and relationships between key features and heart disease.
   - Plotted correlation heatmap for numerical features.

3. **Data Preprocessing & Feature Engineering**
   - Handled missing values.
   - Applied one-hot encoding to categorical variables.
   - Scaled numerical features using StandardScaler.

4. **Model Building & Evaluation**
   - Split data into training and testing sets.
   - Trained and evaluated multiple models:
     - Logistic Regression
     - Decision Tree
     - Random Forest
     - XGBoost Classifier
   - Compared models using accuracy, precision, recall, and F1-score.
   - Visualized confusion matrices for each model.

5. **Model Selection & Saving**
   - Selected the best-performing model based on accuracy.
   - Trained the best model on the full dataset.
   - Saved the trained model using `joblib` for future use.

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- xgboost
- kagglehub
- joblib

Install requirements with:
```sh
pip install pandas numpy matplotlib seaborn scikit-learn xgboost kagglehub joblib