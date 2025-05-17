# Lung Cancer Data Analysis - Exploratory Data Analysis (EDA)

## Description

This project performs an exploratory data analysis (EDA) on a dataset related to lung cancer. 
It uses Python libraries like Pandas, Matplotlib, and Seaborn to load, inspect, and visualize the data, aiming to uncover relationships and patterns between various factors (like age, smoking habits, alcohol consumption) and the incidence of lung cancer.

## Dataset

The analysis uses a CSV file named `lung_cancer_examples.csv`. The dataset contains the following columns:

* `Name`: Name of the individual.
* `Surname`: Surname of the individual.
* `Age`: Age of the individual.
* `Smokes`: A numerical value likely representing the amount or frequency of smoking.
* `AreaQ`: A numerical value (its specific meaning, e.g., air quality index or geographical area, is not defined in the code but is used in analysis).
* `Alkhol`: A numerical value likely representing alcohol consumption.
* `Result`: Binary outcome (0 or 1), where 1 likely indicates a positive lung cancer diagnosis and 0 indicates a negative diagnosis.

## Analysis Performed

The project includes the following types of data analysis and visualizations:

* **Data Loading and Inspection**: Loading the dataset using Pandas and viewing the first few rows (`df.head()`), column names (`df.columns`), and descriptive statistics (`df.describe()`).
* **Relationship Visualization**:
    * Line plots to show the relationship between `Age` and `Result`, with `Smokes` and `Alkhol` as categorical hues.
    * Pair plots (`sns.pairplot`) to visualize pairwise relationships between `Age`, `Smokes`, `AreaQ`, `Alkhol`, and `Result`.
    * Bar plots to show the relationship between `Age` and `Alkhol`, and `Age` and `Smokes`.
* **Distribution Analysis**:
    * Distribution plots (`sns.distplot`) for the `Result` column to see the balance of outcomes.
    * Distribution plots for `Age` among individuals with positive cancer results (`Result == 1`).
    * Distribution plots for `Age` among individuals with negative cancer results (`Result == 0`).
    * Distribution plots for `Alkhol` consumption among individuals with positive cancer results.
* **Correlation and Comparison**:
    * Scatter plots to visualize the relationship between `Age` and `Result`, also with `Smokes` as a hue.
    * Heatmap to show correlations between numerical features (`Age`, `Smokes`, `AreaQ`, `Alkhol`, `Result`).
    * Violin plot to visualize the distribution of `Age` for each `Result` category.

## Libraries Used

* **Pandas**: For data manipulation and loading CSV files.
* **NumPy**: For numerical operations (often used implicitly by Pandas).
* **Matplotlib (`pyplot`)**: For creating static, interactive, and animated visualizations.
* **Seaborn**: For making statistical graphics, built on top of Matplotlib.
