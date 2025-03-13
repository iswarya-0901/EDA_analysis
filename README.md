# EDA_analysis_zomato

## Overview
This project performs an in-depth analysis of the Zomato dataset, covering data preprocessing, exploratory data analysis (EDA), and visualization of key insights. The dataset includes details about restaurants such as their location, cost, ratings, and delivery options. By cleaning and analyzing the data, we extract meaningful patterns and trends.

## Steps Performed

## 1. Data Loading and Initial Exploration
- The dataset is loaded using `pandas.read_csv()` with `latin-1` encoding to handle special characters.
- Initial exploration is done using functions like `df.head()`, `df.tail()`, and `df.info()` to understand the dataset structure and identify missing values.

## 2. Data Cleaning and Preprocessing
- Handling Missing Values: 
  - Categorical columns are filled with the most frequent value using `mode()`.
  - Numerical columns are filled with the median value to maintain consistency.
- Duplicate Removal: 
  - Duplicate rows are identified and removed using `df.drop_duplicates()` to ensure data integrity.
- Outlier Treatment: 
  - Outliers in numerical columns are detected using the IQR (Interquartile Range) method and handled by capping extreme values to an acceptable range.
- Standardizing Categorical Values: 
  - Text values are converted to lowercase and stripped of unnecessary spaces to maintain consistency in analysis.

## 3. Exploratory Data Analysis (EDA)
- Univariate Analysis: 
  - Distributions of numerical variables are visualized using `seaborn.histplot()` and `seaborn.boxplot()`.
  - Frequency distributions of categorical features (e.g., types of restaurants, popular cuisines) are analyzed using bar charts.
- Bivariate Analysis: 
  - Correlation between numerical variables is explored using a heatmap (`sns.heatmap()`).
  - Scatter plots and box plots are utilized to examine relationships between numerical and categorical variables, such as price vs. ratings.
- Multivariate Analysis: 
  - Relationships among multiple variables are studied using `sns.pairplot()`.
  - Grouped comparisons, like rating distributions across different cities, are visualized using box plots and violin plots.

## 4. Data Visualization
- Various `matplotlib` and `seaborn` functions are used to generate visual insights:
  - 'Heatmaps' to analyze correlations between numerical variables.
  - 'Pair plots' to explore relationships among multiple numerical features.
  - 'Box plots & violin plots' to compare cost, ratings, and restaurant types across different locations.

## Summary
This project ensures data integrity by cleaning and preprocessing the dataset before conducting thorough EDA. The visualizations help in understanding restaurant trends, cost distributions, and rating behaviors in different locations. By following a structured approach, we extract actionable insights that aid in decision-making.

## Dependencies
The following Python libraries are required for the analysis:
- `pandas` for data manipulation
- `numpy` for numerical operations
- `matplotlib` and `seaborn` for visualization

## Usage
To analyze and visualize the Zomato dataset, run the script in a Jupyter Notebook or a Python environment. The steps are modular, allowing easy customization for different analysis objectives.



