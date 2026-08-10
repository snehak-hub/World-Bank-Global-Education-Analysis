# World Bank Global Education Analysis

## 📊 Project Overview

**Project Type:** Exploratory Data Analysis (EDA)  
**Contribution:** Individual  
**Author:** Sneha Kumbhar  
**Dataset:** World Bank Education Statistics (EdStats)  
**Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn, Plotly

This project analyzes the **World Bank Education Statistics (EdStats)** dataset to explore global education patterns, differences across countries and regions, education expenditure, literacy, and relationships between education indicators across different years.

The project focuses on data cleaning, preprocessing, exploratory data analysis, visualization, and generating insights that can support education-related decision-making.

---

## 🎯 Problem Statement

The main objectives of this project are:

1. Analyze global education data and identify trends, disparities, and patterns across countries.
2. Explore the World Bank EdStats dataset and generate meaningful insights into global education performance.
3. Compare education-related indicators across countries, regions, and income groups.
4. Understand relationships between education values across different years.
5. Identify areas where data quality and education investment can be improved.

---

## 💼 Business Objective

The business objective is to analyze the World Bank Education Statistics dataset to understand global education trends, compare educational performance across countries, and generate insights that can help governments, researchers, and policymakers make informed decisions about education planning and resource allocation.

---

## 📁 Dataset

The project uses the World Bank **Education Statistics (EdStats)** dataset.

The main dataset used in the notebook is:

- `EdStatsData.csv`

Additional dataset files used during exploration include:

- `EdStatsCountry.csv`
- `EdStatsSeries.csv`

### Dataset Details

- **Rows:** 429,120
- **Columns:** 70 initially
- **Year-wise data:** 1970–2100
- **Coverage:** More than 200 countries and regions
- **Education indicators:** More than 4,000 internationally comparable indicators
- **Total missing values:** 25,978,605 before cleaning

Important identifier columns include:

- `Country Name`
- `Country Code`
- `Indicator Name`
- `Indicator Code`

The dataset contains year-wise numerical education data, with many missing values because not every indicator is available for every country and year.

---

## 🛠️ Technologies Used

### Programming Language
- Python

### Libraries
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly

### Environment
- Google Colab / Jupyter Notebook

---

## 🔄 Project Workflow

The analysis follows these major steps:

```text
Dataset Loading
      ↓
Data Understanding
      ↓
Data Cleaning
      ↓
Missing Value Analysis
      ↓
Data Wrangling
      ↓
Exploratory Data Analysis
      ↓
Visualization
      ↓
Insight Generation
      ↓
Business Recommendations
      ↓
Conclusion
```

---

## 🧹 Data Cleaning & Preparation

The following preprocessing activities were performed:

- Checked dataset shape and structure.
- Inspected columns and data types.
- Checked duplicate records.
- Analyzed missing values.
- Visualized missing values using a heatmap.
- Identified columns containing 100% missing values.
- Removed the `Unnamed: 69` column because it contained no useful information.
- Separated categorical and numerical variables.
- Checked unique values for categorical columns.
- Converted selected year columns to numeric values where required.
- Removed missing observations for specific visualizations where necessary.
- Selected relevant indicators and columns for individual analyses.

---

## 📈 Exploratory Data Analysis & Visualizations

The notebook contains multiple visualizations covering univariate, bivariate, and multivariate analysis.

### 1. Distribution of Education Indicator Values

A histogram is used to understand the distribution of education indicator values for the selected year.

**Purpose:** Understand the spread and concentration of numerical education values.

---

### 2. Box Plot of Education Values

A box plot is used to understand the median, spread, and possible outliers in education indicator values.

**Purpose:** Identify variability and extreme observations.

---

### 3. Top Education Indicators

A bar chart compares the most frequently recorded education indicators.

**Purpose:** Understand which education indicators have greater data coverage.

---

### 4. Education Expenditure by Region

A bar chart compares average government education expenditure across regions.

**Purpose:** Identify differences in education spending between regions.

---

### 5. Education Expenditure by Income Group

A bar chart compares average government education expenditure across income groups.

**Purpose:** Understand how education expenditure varies across different income groups.

---

### 6. Top Countries by Education Expenditure

A bar chart ranks countries based on education expenditure.

**Purpose:** Compare education spending across countries and support benchmarking.

---

### 7. Correlation Heatmap

A correlation heatmap compares education values across selected years:

- 2000
- 2005
- 2010
- 2015
- 2020

**Purpose:** Understand the strength of relationships between education values across years.

---

### 8. Literacy Rate Distribution by Region

A box plot compares literacy rate distributions across regions for 2000.

**Purpose:** Identify regional variation and differences in literacy performance.

---

### 9. Bubble Chart: 2000 vs 2015

A bubble chart compares education values from 2000 and 2015, while bubble size represents the 2010 value.

**Purpose:** Analyze relationships between multiple numerical variables across different years.

---

### 10. Clustered Heatmap

A clustered heatmap groups observations with similar education patterns across selected years.

**Purpose:** Identify similarities and differences in education trends.

---

### 11. Treemap of Education Indicators

A Plotly treemap visualizes the top observations based on 2020 education values using country and indicator hierarchy.

**Purpose:** Provide a compact hierarchical view of education values.

---

### 12. Pair Plot with Region

A pair plot compares 2015 and 2020 education values while using regions as groups.

**Purpose:** Analyze relationships between years and identify regional patterns.

---

## 🔍 Key Insights

The analysis provides the following major insights:

- Education indicators vary significantly across countries and regions.
- Education expenditure differs across regions and income groups.
- Some regions show greater variability in literacy rates than others.
- Education values across selected years show relationships that can help identify longer-term patterns.
- Countries and indicators with larger values can be identified through ranking and hierarchical visualizations.
- Clustering can reveal groups with similar education patterns.
- Missing data is a significant consideration when analyzing global education indicators.
- Differences in education investment and outcomes highlight potential education disparities.

---

## 📌 Business Impact

The insights from this analysis can support:

- Education policy planning.
- Resource allocation.
- Regional benchmarking.
- Identification of underperforming areas.
- Monitoring of education indicators.
- Comparison of education investment across countries and regions.
- Identification of data-quality and reporting gaps.

The analysis also shows that higher education expenditure should not automatically be interpreted as better educational outcomes. Spending should be considered together with indicators such as literacy, enrollment, and school completion.

---

## 💡 Recommendations

Based on the analysis, the following recommendations are proposed:

1. Increase investment in education, especially in countries with low literacy, enrollment, and school completion rates.
2. Focus on improving educational access and quality in low-income and underperforming regions.
3. Use data-driven insights to monitor education indicators and evaluate education policies.
4. Strengthen data collection and reporting processes to reduce missing data.
5. Study successful education policies and practices from high-performing countries.
6. Continuously monitor key education indicators to identify trends and measure progress.

---

## 📂 Project Structure

A recommended GitHub repository structure is:

```text
World-Bank-Global-Education-Analysis/
│
├── World_Bank_Global_Education_Analysis.ipynb
├── README.md
│
├── data/
│   ├── EdStatsData.csv
│   ├── EdStatsCountry.csv
│   └── EdStatsSeries.csv
│
└── images/
    └── charts/
```

> **Note:** The raw World Bank dataset can be large. If you do not want to upload the complete dataset to GitHub, keep the notebook and provide the official dataset source/reference instead.

---

## ▶️ How to Run the Project

### Option 1: Google Colab

1. Open the `.ipynb` file in Google Colab.
2. Upload or connect the required dataset files.
3. Update the dataset path if required.
4. Run the notebook cells from top to bottom.

### Option 2: Jupyter Notebook

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn plotly
```

Then open:

```text
World_Bank_Global_Education_Analysis.ipynb
```

Run the notebook cells sequentially.

---

## 📊 Skills Demonstrated

This project demonstrates practical skills in:

- Data Cleaning
- Data Preprocessing
- Exploratory Data Analysis (EDA)
- Missing Value Analysis
- Descriptive Statistics
- Data Aggregation
- GroupBy Analysis
- Data Visualization
- Correlation Analysis
- Regional Comparison
- Education Expenditure Analysis
- Insight Generation
- Business Recommendations
- Data Storytelling

---

## 🏁 Conclusion

The World Bank Education Statistics (EdStats) project analyzes global education data to identify trends and compare educational performance across countries and regions.

The analysis highlights differences in literacy, education expenditure, and other education indicators. The visualizations make the large dataset easier to understand and help identify patterns, disparities, and areas that may require further attention.

Overall, the project demonstrates how exploratory data analysis and visualization can transform a large education dataset into meaningful insights that can support data-driven decision-making.

---

## 👩‍💻 Author

**Sneha Kumbhar**

GitHub: https://github.com/snehak-hub

---

## ⭐ Project

If you find this project useful, consider giving the repository a ⭐ on GitHub.
