# Smart Customer Segmentation - Mall Customers

This project performs customer segmentation on the Mall Customers dataset using clustering techniques. The goal is to identify distinct customer groups based on features like gender, age, annual income, and spending score.

## Project Structure

- `day5smartsegmentation.ipynb`: Main Jupyter notebook with all code, analysis, and visualizations.

## Steps Performed

1. **Data Loading & Cleaning**
   - Loaded the Mall Customers dataset.
   - Checked for missing values and dropped unnecessary columns.

2. **Exploratory Data Analysis (EDA)**
   - Visualized distributions of age, income, and spending score by gender.
   - Created pair plots and 3D scatter plots for feature relationships.

3. **Clustering & Segmentation**
   - Used KMeans clustering with features like income, spending score, age, and gender.
   - Applied the Elbow Method to determine the optimal number of clusters.
   - Visualized clusters using scatter plots and 3D plots.

4. **Persona Analysis**
   - Analyzed and profiled each cluster to understand customer segments.

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- plotly
- scikit-learn

Install requirements with:
```sh
pip install pandas numpy matplotlib seaborn plotly scikit-learn