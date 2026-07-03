# Wine-Quality-Exploratory-Data-Analysis-EDA


 ## Overview

This project performs a comprehensive Exploratory Data Analysis (EDA) on the WineQT.csv dataset to uncover how physicochemical properties : alcohol content, acidity, pH, and sulphates  influence the quality rating of wine.

# 🎯 Objectives


Clean and audit the dataset for missing values, redundant columns, and inconsistent formatting
Perform univariate analysis to understand feature distributions and skews
Perform bivariate analysis to study relationships between chemical properties and wine quality
Build a correlation matrix to identify the strongest statistical drivers of wine quality
Extract actionable insights that could inform future predictive modeling


# 🛠️ Tools & Libraries


Python
Pandas – data manipulation and cleaning
NumPy – numerical operations
Matplotlib – data visualization
Seaborn – statistical plotting


# 🔍 Analytical Workflow


Data Loading – Imported the WineQT.csv dataset into a Pandas DataFrame and verified its dimensions
Structural Auditing – Previewed data with .head() and inspected data types with .info()
Missing Data Diagnostics – Confirmed zero missing values across all features
Column Normalization – Dropped the non-chemical Id index column and standardized column headers
Univariate Analysis – Visualized distribution of quality (target) and alcohol content; examined volatile_acidity outliers via boxplot and pH distribution via histogram
Bivariate Analysis – Compared alcohol and volatile_acidity across quality tiers; analyzed mean sulphates by quality group and the relationship between citric_acid and volatile_acidity
Correlation Matrix – Generated a full Pearson correlation heatmap across all features


# 📊 Key Insights

FindingCorrelation with QualityAlcohol content is the dominant quality driver — premium wines (rated 7–8) average above 11.5% alcohol+0.48Volatile acidity is the primary quality inhibitor — high-quality wines stay below 0.40 g/dm³-0.41Sulphates play a preservation role — levels rise steadily with quality due to antimicrobial/antioxidant effects+0.26Fixed acidity vs. density shows a strong structural relationship affecting body and mouthfeel+0.68

Additional observation: The target variable (quality) is heavily imbalanced — most samples cluster around scores 5–6, while extreme scores (3 and 8) are rare. This class imbalance would need to be addressed before training any future predictive ML model on this data.

# 📁 Repository Structure

├── WineQuality_EDA_Rafia_Rameen.ipynb   # Main analysis notebook
├── correlation_matrix_heatmap.png        # Exported correlation heatmap
└── README.md

# 🚀 How to Run


Clone this repository
Open WineQuality_EDA_Rafia_Rameen.ipynb in Jupyter Notebook or Google Colab
Ensure WineQT.csv is placed in the same directory (or update the file path)
Run all cells sequentially


# 📌 Dataset Source

Wine Quality Dataset (WineQT) — commonly sourced from Kaggle's Wine Quality dataset collection.


Part of my AI/ML internship assignments — focused on building strong data analysis and visualization fundamentals.
