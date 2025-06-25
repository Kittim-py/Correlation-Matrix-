Correlation Analysis & Heatmap Visualization in Python

This script allows you to perform correlation analysis on a CSV dataset, visualize the results with a significance-annotated heatmap, and generate a correlation bar plot with a target variable.

---

Features
1. Computes Pearson correlation coefficients
2. Calculates p-values for statistical significance
3. Heatmap visualization with significance symbols:
4. `•` (p ≤ 0.05), `••` (p ≤ 0.01), `•••` (p ≤ 0.001)
5. Bar graph showing correlation of features with a selected target column
6. Saves correlation and p-value matrices as CSV

Requirements

Make sure you have the following Python libraries installed:

bash
pip install pandas numpy matplotlib seaborn scipy
```

Input

A CSV file with numerical data
Manual input of:

`input_columns`: List of columns to consider for correlation analysis
`target_column`: Column name used for the bar chart visualization


Usage

1. Edit the script:

   Update these variables:

   ```python
   dataset = pd.read_csv('your_data.csv')  # Replace with your actual CSV path

   input_columns = ['column1', 'column2', 'column3', ...]  Exclude the target column

   target_column = 'target_column_name'
   ```

2. Run the script:

   ```bash
   python correlation_analysis.py
   ```

3. Enter a title when prompted for the heatmap chart.

5. View visualizations:

Heatmap with annotated correlation values and significance
Bar plot showing correlation of each input variable with the target

6. Check outputs**:

Two CSVs will be saved:

`correlation_matrix.csv`
  `p_value_matrix.csv`

 ⚠️ Notes

* Works only with **numerical columns**
* Make sure **no missing values** are present or handle them before analysis
* Target column should **not be included** in `input_columns`


## ✍️ Author
Arindam Roy 

Developed for scientific/statistical analysis using Python.
