### DatafestPSU 2025 - Awards in Best Use of External Resources
**We are not allowed to keep the dataset provided from ASA. Findings are documented below.**


### 👥 Team Contributions

- **Seokhyeon Bae**  
  - **Presenter**: Delivered the final presentation.  
  - **Data Analysis**: Analyzed datasets from ASA and external sources.  
  - **Economic Insights**: Selected relevant data sources and constructed the regression models with interpretation.  
  - **Data Visualization**: Used **Stata** to visualize regression outputs and trends.

- **Hyunwoo Jang**  
  - **Data Cleaning**: Preprocessed data using **R** and **Jupyter Notebook**.  
  - **Data Analysis**: Performed statistical analysis on ASA and external datasets.  
  - **Economic Insights**: Collaborated in selecting variables and interpreting regression results.  
  - **Data Visualization**: Visualized findings using **R**.

- **Hanna Oh**  
  - **Data Cleaning**: Processed raw data using **Jupyter Notebook** for analysis readiness.  
  - **Presentation Design**: Created the final presentation slides with clear economic interpretation for the presenter.

- **Hojin Yoon**  
  - **Data Analysis**: Contributed to the analysis of ASA and external datasets.  
  - **Documentation**: Maintained detailed project notes and ensured the team stayed on track throughout development.


### Project: Rent Cost Analysis Across U.S. Regions

#### This project investigates which factors most strongly influence rent prices across the U.S., using a multi-level data analysis approach. 
---

### 🔍 Analytical Framework

We analyzed rent determinants at three spatial scales:

1. **State-Level Analysis**:  
   - Focused on macroeconomic variables (e.g., unemployment, CPI, corporate presence).
   - Adjusted values using CPI to control for price level differences across states.
   - Final model included:  
     `count`, `total`, `key_industry_rate`, and `cpi`.  
   - Achieved strong explanatory power (R² = 0.8258, adj. R² = 0.7635).

2. **ZIP Code-Level Analysis**:  
   - Offered finer regional insights by clustering nearby ZIP codes.
   - Highlighted the growing importance of `cbd_rate` (central business district concentration) at the local scale.
   - Final model included:  
     `count`, `key_industry_rate`, `cbd_rate`, and `cpi`  
   - All variables were statistically significant (p < 0.01), R² = 0.5932.

3. **Quality-of-Life Variables**:  
   - Included factors such as crime rate, education, health, and retail access.
   - Most showed weak correlation with rent; only `cbd_rate` and `education` had a noticeable effect.
   - Concluded that **economic factors**, not quality-of-life, are the primary rent drivers.

---

### Key Insights

- **Corporate presence** and **industry type** (engineering, tech, finance, business) are strongly associated with higher rent.
- **Urban centrality** (`cbd_rate`) becomes increasingly significant at localized levels.
- **Income and population change**, while intuitive, did not have strong statistical significance in explaining rent.
- **Quality of life factors**, despite common assumptions, had minimal effect on rent variation.

---

### External Data Sources (Selected)

- CPI: [BLS](https://www.bls.gov/regions/subjects/consumer-price-indexes.htm)  
- Income: [FRED](https://fred.stlouisfed.org/series/MEHOINUSA646N)  
- Population: [U.S. Census](https://www.census.gov/library/visualizations/2023/comm/percent-change-state-population.html)  
- Education & Health: [WalletHub](https://wallethub.com/edu/e/states-with-the-best-schools/5335), [America’s Health Rankings](https://www.americashealthrankings.org/)  
- Retail Locations: Kaggle (Costco, Walmart, Target)  
- Crime Data: [FBI UCR](https://cde.ucr.cjis.gov/LATEST/webapp/#/pages/home)

---

### Conclusion

Our analysis shows that **rent prices are primarily driven by economic variables** such as corporate density, industrial specialization, and CPI—not lifestyle or quality-of-life metrics. These insights can help guide urban planning, corporate site selection, and housing policy decisions.
The presenetation will be availale soon.

---

### Reflection
This hand-on experience as a data scientist and economist was difficult, but strendous. When we were given with the dataset, we did not know how to utilize those data because there was no teammate with real-world experience in data. 
As we develop our ideas, we realized how important the economic insight is; we needed to choose which data and models to use, consider how to implement this data into our models, and predict how it will turn out. 
