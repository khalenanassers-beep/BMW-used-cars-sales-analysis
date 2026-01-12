# Which used BMW Cars makes more sense? 

## 📘 Project Scenario
A small business owner needs to help him understand his current inventory database of used BMW cars. His main question was straightforward but strategically important:
“Should I focus on acquiring more Diesel cars or Gasoline cars for the next quarter?”

To answer this, a full Exploratory Data Analysis (EDA) of his dataset, focusing specifically on:
- Mileage (how used the cars are)
- Fuel type (Diesel vs Gasoline)
- Market activity (which combinations appear more often, indicating higher demand)
  
This analysis helps the business owner make data‑driven purchasing decisions for the upcoming quarter.

### 📁Dataset
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

### 🔧Tools & Libraries

The analysis is performed in R Studio using:
- tidyverse
- janitor
- skimr
- summarytools
- GGally
- corrplot
- ggridges

### 📊Analysis Steps

**1.Data Loading & Cleaning**
- Import CSV
- Clean column names (not need in this case)
- Inspect structure and missing values (no missing values, which is not common)
  
**2. Summary Statistics**
For each numeric variable:
- Mean
- Median
- Mode
- Variance
- Range
- Standard deviation
  
**3. Distributions**
Histograms for all numeric variables.

**4. Categorical Analysis**
Bar charts for:
- Model
- Transmission
- Fuel type
  
**5. Correlation Analysis**
Two types:
- Heatmap (corrplot)
- Scatterplot matrix with histograms (GGally::ggpairs)
  
**6. Boxplots**
- Boxplots for each numeric variable
- Boxplots of numeric variables by fuel type

## **7. Dive on Mileage and Fuel Type**

- Number of Listings by Fuel Type

- Correlation Tests
  - Mileage ↔ Price (Pearson test)  
  - Mileage ↔ Fuel Type (binary)  
  - Price ↔ Fuel Type (binary)

- Welch Paired t‑Tests (Diesel vs Petrol)
  - Mileage t‑test  
  - Price t‑test  

- Comparing Graphs
  - Heatmap of mileage group × fuel type  
  - Boxplot: price by fuel type  
  - Boxplot: mileage by fuel type

## **8. Business Report**

