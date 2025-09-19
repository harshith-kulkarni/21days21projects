# QUESTIONS ARE WRITTEN IN QSNS.MD


# Netflix Dataset Exploratory Data Analysis (EDA)

This project performs an exploratory data analysis (EDA) on the Netflix dataset as part of the "21 Days 21 Projects" challenge. The analysis covers data cleaning, feature engineering, univariate, bivariate, and multivariate analysis, as well as outlier detection and automated profiling.

## Project Structure

- `day2netflix.ipynb`: Main Jupyter notebook containing all code and analysis steps.
- `Readme.md`: Project documentation (this file).

## Steps Performed

1. **Data Loading**
   - The Netflix dataset is loaded using pandas.

2. **Data Cleaning**
   - Handled missing values in relevant columns.
   - Converted data types where necessary.

3. **Univariate Analysis**
   - Visualized categorical features using count plots.
   - Visualized numerical features using histograms and boxplots.

4. **Bivariate Analysis**
   - Explored relationships between features using bar plots and correlation matrices.

5. **Outlier Detection**
   - Used boxplots to detect outliers in numerical columns.

6. **Feature Engineering**
   - Created new features (e.g., extracting year from date columns, categorizing content types).

7. **Multivariate Analysis**
   - Used categorical plots and heatmaps to analyze interactions between multiple features.

8. **Automated Profiling**
   - Generated a comprehensive profiling report using YData Profiling (if applicable).

## How to Run

1. Open `day2netflix.ipynb` in Jupyter Notebook or VS Code.
2. Run all cells to execute the analysis.

## Requirements

- Python 3.x
- pandas
- seaborn
- matplotlib
- numpy
- ydata-profiling (optional, for profiling report)

Install requirements with:
```sh
pip install pandas seaborn matplotlib numpy ydata-profiling