🚗 BMW Used Cars — Exploratory Data Analysis (EDA)
This project explores a dataset of BMW used cars to uncover pricing patterns, performance characteristics, and model‑specific insights. The analysis includes data cleaning, summary statistics, distributions, correlation analysis, and boxplots.
📁 Dataset
The dataset contains BMW car listings with variables such as:
- Model
- Price
- Mileage
- Year
- Transmission
- Fuel type
- Engine size
- MPG
- Tax
Source: Kaggle dataset (https://www.kaggle.com/datasets/thedrzee/bmw-carsdataset?resource=download)

🔧 Tools & Libraries
The analysis is performed in R Studio using:
- tidyverse
- janitor
- skimr
- summarytools
- GGally
- corrplot
- ggridges

📊 Analysis Steps
1. Data Loading & Cleaning
- Import CSV
- Clean column names (not need in this case)
- Inspect structure and missing values (no missing values, which is not common)
2. Summary Statistics
For each numeric variable:
- Mean
- Median
- Mode
- Variance
- Range
- Standard deviation
3. Distributions
Histograms for all numeric variables.
4. Categorical Analysis
Bar charts for:
- Model
- Transmission
- Fuel type
5. Correlation Analysis
Two types:
- Heatmap (corrplot)
- Scatterplot matrix with histograms (GGally::ggpairs)
6. Boxplots
- Boxplots for each numeric variable
- Boxplots of numeric variables by BMW model
