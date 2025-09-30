# Customer Churn Prediction - Feature Engineering & Model Comparison

This project explores the impact of feature engineering and feature selection on customer churn prediction for a telecommunications company. The notebook demonstrates how to build, compare, and improve machine learning models using both raw and engineered features.

## Project Structure

- `day7customerchurning.ipynb`: Main Jupyter notebook with all code, analysis, and results.

## Steps Performed

1. **Project Objective & Concepts**
   - Demonstrated the importance of feature engineering for model performance.
   - Covered advanced data cleaning, feature creation, and model evaluation.

2. **Data Loading & Cleaning**
   - Loaded the Telco Customer Churn dataset.
   - Addressed missing values and data type inconsistencies.

3. **Baseline Model**
   - Built a logistic regression model using only the original features.
   - Established benchmark performance metrics.

4. **Feature Engineering**
   - Created new features: tenure bins, service counts, ratios, and combined categories.
   - Simplified categorical variables for better interpretability.

5. **Enhanced Model**
   - Built and evaluated models using engineered features.
   - Compared performance to the baseline.

6. **Feature Selection**
   - Applied methods like SelectFromModel and RFE to select the most important features.
   - Compared model performance with selected features.

7. **Model Comparison**
   - Evaluated Logistic Regression, Random Forest, Gradient Boosting, and SVM.
   - Compared results on both full and feature-selected datasets.

8. **Hyperparameter Tuning**
   - Used GridSearchCV to optimize model parameters for top-performing models.

9. **Analysis & Reporting**
   - Summarized results in tables and visualizations.
   - Discussed which features and techniques were most effective.

## Key Findings

- Feature engineering improved the model's ability to predict churn, especially for the minority class.
- Feature selection (with the tested methods) did not significantly improve performance over the enhanced model.
- Logistic Regression, Gradient Boosting, and SVM performed similarly; Random Forest was slightly less effective.
- Further improvements may require more advanced feature engineering or techniques for handling class imbalance.

## How to Run

1. Open `day7customerchurning.ipynb` in Jupyter Notebook or VS Code.
2. Run all cells in order to reproduce the analysis and results.

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

Install requirements with:
```sh
pip install pandas numpy matplotlib seaborn scikit-learn