# Market Basket Analysis (Association Rule Mining)

## Overview
This project applies **Market Basket Analysis** to real-world online retail transaction data in order to uncover **frequent itemsets** and **association rules** using the **Apriori algorithm**.  
The goal is to identify products that are frequently purchased together and translate these patterns into **actionable business insights** such as cross-selling opportunities and product bundling strategies.

---

## Dataset
- **Source:** UCI Machine Learning Repository – Online Retail Dataset  
- **Period:** December 2010 – December 2011  
- **Description:** Transactional data from a UK-based online retailer selling gift items  
- **Size:** ~540,000 transaction records  

---

## Methodology

### Data Cleaning & Preparation
- Removed canceled transactions and zero-quantity records  
- Filtered invalid prices and missing descriptions  
- Handled missing customer IDs  
- Converted transactions into a format suitable for association rule mining  

### Exploratory Analysis
- Identified the most frequently purchased products  
- Visualized item frequencies to understand purchasing behavior  

### Association Rule Mining
- Applied the Apriori algorithm  
- Tuned support and confidence thresholds to extract meaningful rules  
- Evaluated rules using **support**, **confidence**, and **lift**  

### Interpretation & Visualization
- Selected high-confidence rules  
- Visualized the strongest associations  
- Interpreted rules in a business context  

---

## Key Findings
- Certain products (e.g., themed gift items) show strong co-purchasing behavior  
- High-lift rules indicate non-random, meaningful associations  
- Identified item combinations suitable for:
  - Cross-selling  
  - Product bundling  
  - Targeted promotions  

---

## Tools & Technologies
- **Language:** R  
- **Libraries:** arules, arulesViz, tidyverse, viridis  
- **Techniques:** Apriori Algorithm, Association Rule Mining, Data Cleaning, Visualization  

---

## How to Run the Project

### Clone the repository
```bash
git clone https://github.com/yourusername/market-basket-analysis.git
```
## How to Run the Project

### Install required R packages
```r
install.packages(c("tidyverse", "arules", "arulesViz", "viridis", "readxl"))
```
### Download the dataset
Download **Online Retail.xlsx** from the UCI Machine Learning Repository and place it in the project root directory.

### Run the analysis
- Open the `.Rmd` file in RStudio  
- Click **Knit** to generate the HTML report  

### View results
- Open the generated `.html` file in a web browser to explore the full analysis and visualizations
