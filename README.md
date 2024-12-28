# 🏡 Housing in Brazil – Real Estate Data Analysis  

## 📋 Project Overview  
This project analyzes real estate data from Brazil to uncover regional differences in the housing market. A key focus is on the southern region, exploring the relationship between home size and price.  

---

## 🗂️ Data  
The project uses two CSV files:  
- **brasil-real-estate-1.csv** – Includes property data (with prices in USD)  
- **brasil-real-estate-2.csv** – Contains property data (with prices in BRL)  

---

## 🛠️ Tools & Libraries  
- **Python** (pandas, matplotlib)  
- **Jupyter Notebook**

---

## 📊 Analysis Breakdown  

### 1. Data Import & Inspection  
- Imported and inspected both datasets to understand structure and missing values.  
- Dropped rows with null latitude-longitude data (about 10% of the dataset).  
- Extracted **latitude and longitude** into separate columns for spatial analysis.  

### 2. Data Cleaning  
- Extracted **state names** from hierarchical location columns.  
- Converted price columns from **strings to float** by removing dollar signs and commas.  
- **Price in BRL** was converted to USD using the exchange rate of **1 USD = 3.19 BRL**.  

### 3. Merging Datasets  
- After cleaning, the two datasets were concatenated into a single dataframe for further analysis.  

---

## 🔍 Exploratory Data Analysis (EDA)  
- **Descriptive Statistics** – Summary of home sizes and prices.  
- **Visualizations**  
  - **Histogram** – Distribution of home prices (right-skewed).  
  - **Boxplot** – Distribution of home sizes.  
  - **Bar Chart** – Mean home price by region.  
  - **Scatterplot** – Relationship between area and price in **Rio Grande do Sul**.  

---

## 📈 Key Findings  
- **Regional Differences** – Southeast and South had the highest average home prices.  
- **South Region Analysis**:  
  - Homes in **Rio Grande do Sul** had the largest representation.  
  - Price and area showed **slight positive correlation** across all southern states.  
  - **Correlation Coefficients**:  
    - Paraná: **0.54**  
    - Rio Grande do Sul: **0.58**  
    - Santa Catarina: **0.51**

