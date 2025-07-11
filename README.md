# Statistical-and-Predictive-Modeling

**Data Analysis using Python Modelling**

Developed a Python-based energy usage analysis pipeline using IQR outlier detection, cleaned 768-row dataset using Tukey’s rule, and prepared it for predictive modeling through structured data profiling and cleansing.

**1. Library Imports and Setup**

Imported core data analysis and visualization libraries:

numpy, pandas, matplotlib.pyplot, seaborn

Set up inline plotting for visual output in notebook

**2. Data Loading and Initial Exploration**

Dataset: EnergyUse-Heating.csv

Size: 768 rows × 9 columns (X1–X8 as features, Y as target)

Action: Loaded into a DataFrame using pd.read_csv(), previewed with df.head()


**3. Descriptive Statistics (Data Profiling)**

Used df.describe() to analyze:

Central tendency: mean, median

Spread: std, min, max, quartiles (25%, 75%)

Insight: Identified skewness, variation in energy usage features


**4. Custom Outlier Detection with Tukey Method**

Defined a reusable function detect_outliers() using:

Q1, Q3, and IQR (Interquartile Range)

Tukey’s Rule: outlier = value < Q1 – 1.5×IQR or > Q3 + 1.5×IQR

Applied it across all features (X1 to X8), excluding the target Y


 **5. Identifying and Removing Outliers**


Created a list of rows containing multiple extreme outliers

Result:

Identified multiple records with ≥2 extreme outlier values

Removed them to create a cleaner subset good_data


**6. Cleaned Dataset Overview**

Used .info() and .reset_index() on good_data

Result:

Final dataset size maintained at 768 entries after reset

Ensured all columns were clean and of correct dtype (e.g., float64, int64)



| Skill Area                 | Demonstrated Work                                             |
| -------------------------- | ------------------------------------------------------------- |
| **Data Profiling**         | `describe()`, summary stats                                   |
| **Custom Function Design** | Defined scalable outlier detection logic                      |
| **Statistical Thinking**   | Applied Tukey’s Rule for multi-feature outlier identification |
| **Data Cleaning**          | Filtered and reset index for modeling readiness               |
| **Python Scripting**       | Looping, conditionals, Counter from `collections`             |
| **EDA Foundations**        | Built a solid base for regression/forecasting                 |


Engineered and standardized eight building and operational features to prepare data for modeling.

Developed and optimized regularization models (LASSO, Ridge, Elastic Net) in Python (Jupyter Notebook) to forecast building heating load.

Evaluated models using cross-validation and key metrics (Adjusted R², MAE, RMSE), extracting actionable insights from each approach.

Selected the best-performing model based on predictive accuracy and interpretability, recommending targeted next steps to enhance model usability.


