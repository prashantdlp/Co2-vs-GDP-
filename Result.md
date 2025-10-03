# GDP vs CO₂ Emissions Analysis

**Role:** Self Project  
**Duration:** Aug – Sep 2024  

## Objectives

- Analyze the relationship between economic growth (GDP) and CO₂ emissions for major countries.  
- Identify patterns of decoupling between GDP growth and emissions.  
- Perform regression and correlation analysis to quantify relationships.

## Datasets Used

- World Bank / OWID CO₂ dataset (1991–2020).  
- Key variables: `country`, `year`, `GDP`, `CO₂ emissions`, `CO₂ per capita`, `CO₂ per GDP`, and main emission sources (`coal`, `oil`, `gas`, `cement`).

## Methodology

1. **Data Cleaning**
   - Selected relevant columns and filtered years 1991–2020.  
   - Converted numeric columns and handled missing values.  

2. **Exploratory Analysis**
   - Visualized GDP vs CO₂ trends for multiple countries using scatter plots.  
   - Computed CO₂ per GDP to analyze carbon intensity trends.

3. **Statistical Analysis**
   - Performed **linear regression** of GDP vs CO₂ emissions for each country.  
   - Computed **Pearson correlation coefficients** to measure strength and direction of relationships.

## Key Results

| Country        | Correlation (r) | p-value | Insight |
|----------------|----------------|---------|---------|
| China          | 0.95           | 0.000   | Strong positive correlation; GDP growth drives CO₂ emissions. |
| India          | 1.00           | 0.000   | Very strong positive correlation; emissions increase with GDP. |
| Brazil         | 0.97           | 0.000   | Strong positive correlation; economic growth coupled with emissions. |
| United States  | -0.09          | 0.625   | No significant correlation; emissions plateau despite GDP growth. |
| Germany        | -0.93          | 0.000   | Strong negative correlation; GDP growth decoupled from CO₂ emissions. |

- Regression plots showed fitted linear trends for GDP vs CO₂ for each country.  
- Carbon intensity trends visualized CO₂ per GDP over time to identify decoupling in developed countries.

## Conclusions / Insights

- **Developing economies** (China, India, Brazil) exhibit strong positive correlation, indicating GDP growth is associated with higher emissions.  
- **Developed economies** (Germany, US) show decoupling: economic growth occurs with stable or decreasing emissions.  
- **Policy implication:** Renewable energy adoption, efficiency measures, and regulations in mature economies are effective in reducing carbon intensity.

## Tools & Technologies

- **Python:** Pandas, NumPy, Matplotlib, Scikit-learn (Linear Regression), SciPy (Pearson correlation).  
- **Data Sources:** World Bank / OWID CO₂ datasets (CSV).
