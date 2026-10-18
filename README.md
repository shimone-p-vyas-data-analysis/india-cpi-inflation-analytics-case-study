# Excel Case Study: India Consumer Price Index Inflation
*Case Study Completion Date:* *April 27, 2026*

![Year-on-Year inflation trend analysis](03-yoy-inflation-peak.png) 

## **Data and Repository Restrictions**

> To maintain academic integrity for ongoing peer cohorts, the institutional source data and my final .xlsx workbook are withheld from the repository.

> Visual assets are watermarked for portfolio integrity. 

## Case Study Overview 
Comprehensive Excel Analytics Project on India's Consumer Price Index Inflation. 
- Comprises raw data cleaning, **diagnostic analysis** and **visualizations**.
- Utilized a **Multi-Horizon time-series analysis : Year-on-Year (Y-o-Y), Month-on-Month (M-o-M)** to track trends.
- Extracted **macroeconomic insights**.
- **Correlated the Imported global crude oil prices** with the rest of the individual categories.
- Isolated the underlying Food **supply shocks**.

## Data Source
- Utilized an officially provisioned case study dataset curated from an open-source **GOI** public data repository containing relevant records from **January 2013 - May 2023**.
- The **imported Crude oil values** from **January 2021 - May 2023** for the **Rural+Urban** sector were sourced directly from the internet. The values presented are based on historical market records.

## Data Cleaning
* Cleaned and structured 373 rows of data.
* Performed deletion of 3 rows of May 2020 (0.08% of the dataset) as they were 'NA'.
* Cleaned missing data fields by standardising 'NA' and string hyphens '-' to 0, thus eliminating calculation breaks.
* For Rural Sector in April 2020, linear interpolations were computed.
* **`Linear interpolation: April 2020 = March 2020 + June 2020 / 2`**
* Used **`TRUNCATE()`** function to 1 decimal place to maintain data consistency.

## Data Analysis Report Sequence
| File Order | Description |
| :--- | :--- |
| **1. `food-contribution.png`** | Upto **50%** contribution to inflation across sectors by the major and broad **Food** category |
| **2. `yoy-inflation.png`** | **Y-o-Y inflation%** computed |
| **3. `yoy-inflation-peak.png`** | **2022** highlighted as the period of peak inflation |
| **4. `mom-inflation-deflation-peak.png`** | **June 2022** had the **highest M-o-M inflation%** of **1.03** while **December 2022** saw a **M-o-M deflation%** of **-0.58** |
| **5. `food-breakdown-sub-categories.png`** | **Spices** contributing upto **16.6%**, is the largest within the Food category |
| **6. `correlation-icon-set-classification.png`** | Calculation of Correlation for the Imported Crude Oil Prices with all the sub-categories |
| **7. `strong-correlation-scatterplot.png`** | Strong Correlation of **0.77** between the Imported Crude Oil Prices and the Meat and Fish category |
