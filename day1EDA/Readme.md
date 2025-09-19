# Titanic Dataset Exploratory Data Analysis (EDA)

This project performs an exploratory data analysis (EDA) on the Titanic dataset as part of the "21 Days 21 Projects" challenge. The analysis covers data cleaning, feature engineering, univariate, bivariate, and multivariate analysis, as well as outlier detection and automated profiling.

## Project Structure

- `day1EDA.ipynb`: Main Jupyter notebook containing all code and analysis steps.
- `titanic.html`: Automated profiling report generated using YData Profiling.
- `Readme.md`: Project documentation (this file).

## Steps Performed

1. **Data Loading**
   - The Titanic dataset is cloned from [GeeksforGeeks 21-Days-21-Projects-Dataset](https://github.com/GeeksforgeeksDS/21-Days-21-Projects-Dataset).
   - Data is loaded using pandas.

2. **Data Cleaning**
   - Handled missing values in `Age`, `Cabin`, and `Embarked`.
   - Created a binary feature `Has_Cabin` and dropped the original `Cabin` column.

3. **Univariate Analysis**
   - Visualized categorical features using count plots.
   - Visualized numerical features (`Age`, `Fare`) using histograms.

4. **Bivariate Analysis**
   - Explored relationships between features and survival using bar plots and facet grids.

5. **Outlier Detection**
   - Used boxplots to detect outliers in the `Fare` column.

6. **Feature Engineering**
   - Created new features: `familysize`, `alone`, and extracted `Title` from passenger names.
   - Grouped rare titles and visualized survival rates by title.

7. **Multivariate Analysis**
   - Used categorical plots and violin plots to analyze interactions between multiple features.
   - Generated a correlation heatmap.

8. **Automated Profiling**
   - Generated a comprehensive profiling report using YData Profiling (`titanic.html`).

## How to Run

1. Clone the dataset:
   ```sh
   git clone 'https://github.com/GeeksforgeeksDS/21-Days-21-Projects-Dataset'
   ```

2. Open `day1EDA.ipynb` in Jupyter Notebook or VS Code.

3. Run all cells to execute the analysis and generate the profiling report.

## Requirements

- Python 3.x
- pandas
- seaborn
- matplotlib
- numpy
- ydata-profiling

Install requirements with:
```sh
pip install pandas seaborn matplotlib numpy ydata-profiling
```

## Output

- **Notebook:** Step-by-step EDA in [`day1EDA.ipynb`](day1EDA.ipynb)
- **Profiling Report:** Interactive HTML report in [`titanic.html`](titanic.html)

---

*This project is part of the 21 Days 21 Projects challenge.*