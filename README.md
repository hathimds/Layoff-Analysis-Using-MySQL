# 📊 Layoff Analysis Using SQL

## 📌 Objective
To analyze global tech industry layoffs using structured SQL queries — starting from **data cleaning**, followed by **exploratory data analysis** — to discover patterns in layoffs across time, industries, and companies.

---

## 🧰 Tools Used
- MySQL
- SQL Window Functions
- CTEs (Common Table Expressions)
- Aggregate functions and grouping

---

## 🗃️ Dataset
- **Source**: `layoffs.csv` (Kaggle)
- **Features**: Company, Location, Industry, Date, Total Laid Off, Percentage Laid Off, Country, Funds Raised, etc.
- **Total Rows**: ~2300+ entries

---

## 🧹 Data Cleaning Steps (Summary)
- Removed duplicates using `ROW_NUMBER()` window function
- Standardized text fields (e.g., trimming whitespace, consistent labels like "Crypto")
- Converted date format to proper SQL `DATE` type
- Imputed missing industry data based on company names
- Deleted irrelevant rows with null values in both `total_laid_off` and `percentage_laid_off`

> See: [`data_cleaning.sql`](./SQL/data_cleaning.sql)

---

## 📊 Exploratory Data Analysis (Key Queries)
- Maximum layoffs in a single event
- Companies with 100% layoffs and their funding
- Top 10 companies by total laid-off employees
- Year-wise and month-wise layoffs
- Industry-wise and country-wise layoff distributions
- Rolling monthly layoffs using window functions
- Top 5 companies with the highest layoffs each year

> See: [`exploratory_data_analysis.sql`](./SQL/exploratory_data_analysis.sql)

---

## 📈 Key Insights
- Companies like **Meta**, **Amazon**, and **Google** saw massive layoffs in specific years.
- The **Technology and Retail** industries were among the hardest hit.
- The **United States** had the highest number of layoffs.
- A significant spike in layoffs was observed during late 2022 to early 2023.
- Layoffs surged despite some companies raising millions in funding.

---

## 📂 Project Structure
```
Layoff-Analysis-Using-MySQL/
│
├── SQL/
│   ├── data_cleaning.sql
│   └── exploratory_data_analysis.sql
└── README.md
```

---

## 🚀 Future Scope
- Integrate Power BI dashboard for visual storytelling
- Add predictive analysis based on funding + layoffs
- Publish blog or LinkedIn post summarizing the project

---

## 🧠 Author
**Haathim Manaf**  
_Passionate Data Science & Data Analysis Learner | SQL • Power BI • Python_
