# HR Analytics Dashboard — Excel

An advanced, interactive HR Analytics Dashboard built entirely in Microsoft Excel. Analyzes employee attrition patterns across **1,470+ employee records**, identifying key drivers such as job role, education field, department, and satisfaction levels.

---

## 📊 Dashboard Preview

| KPI | Value |
|-----|-------|
| **Total Headcount** | 1,470 |
| **Active Employees** | 1,233 |
| **Attrition Count** | 237 |
| **Attrition Rate** | 16.12% |

### Full Dashboard View
![Full Dashboard](https://github.com/sivasankar3002/HR-Analytics-Dashboard-Excel/blob/main/screenshots/Screenshot%202026-07-11%20223854.png)

### Data
![Data](https://github.com/sivasankar3002/HR-Analytics-Dashboard-Excel/blob/main/screenshots/Screenshot%202026-07-11%20223929.png)

### Attrition Analysis
![Attrition Analysis](https://github.com/sivasankar3002/HR-Analytics-Dashboard-Excel/blob/main/screenshots/Screenshot%202026-07-11%20224000.png)

### Income Analysis
![Income Analysis](https://github.com/sivasankar3002/HR-Analytics-Dashboard-Excel/blob/main/screenshots/Screenshot%202026-07-11%20224028.png)

### Review
![Review](https://github.com/sivasankar3002/HR-Analytics-Dashboard-Excel/blob/main/screenshots/Screenshot%202026-07-11%20224038.png)

---


## ✨ Key Features & Advanced Techniques

### Dynamic KPI Dashboard
- **4 interactive KPI cards** with color-coded accent bars (green for active, red for attrition, amber for rate)
- **7 high-resolution embedded charts** — donut, horizontal bar, column, area, funnel, and comparison charts
- Professional **Bloomberg-style dark terminal aesthetic** with a cohesive color system

### Data Processing & ETL
- Cleaned and transformed raw IBM HR dataset (44 columns → 34 meaningful fields)
- Derived calculated fields: `Attrition Flag` (binary), `Age Band` (categorical grouping)
- Consolidated employee demographics, satisfaction surveys, and performance ratings into a single standardized template

### Multi-Dimensional Attrition Analysis (10 Dimensions)
| Dimension | Insight Type |
|-----------|-------------|
| Department | Attrition count, rate, and active split by HR / R&D / Sales |
| Job Role | Breakdown across 9 roles (Sales Exec, Lab Tech, Research Scientist, etc.) |
| Education Field | 6 fields including Life Sciences, Medical, Marketing, Technical Degree |
| Age Band | 5 groups: Under 25, 25–34, 35–44, 45–54, Over 55 |
| Marital Status | Single, Married, Divorced |
| Gender | Male vs Female |
| Overtime | Impact of overtime on attrition |
| Business Travel | Travel frequency vs turnover |
| Job Satisfaction | 4-level satisfaction scale analysis |
| Environment Satisfaction | Workplace environment rating impact |

### Advanced Conditional Formatting (4 Types)
1. **Data Bars** — Visual in-cell bars on Monthly Income column (min–max scaling)
2. **Color Scale** — 3-color gradient on Age column (light blue → teal → deep navy)
3. **Formula-Based Rule** — Entire row highlights red when `Attrition = "Yes"`
4. **Cell-Based Rules** — Department attrition rates: red (>20%), amber (>16%), with automatic font styling

### Charts & Visualizations (11 Total)
| # | Chart | Type | Location |
|---|-------|------|----------|
| 1 | Attrition by Marital Status | Donut | Dashboard |
| 2 | Attrition Rate by Department | Column (color-coded) | Dashboard |
| 3 | Attrition Count by Job Role | Horizontal Bar | Dashboard |
| 4 | Attrition Count by Education Field | Horizontal Bar | Dashboard |
| 5 | Attrition Rate by Age Group | Area | Dashboard |
| 6 | Attrition Rate by Job Satisfaction | Column (funnel-style) | Dashboard |
| 7 | Attrition Rate by Overtime Status | Column | Dashboard |
| 8 | Attrition Share by Department | Pie | Analysis |
| 9 | Attrition Count by Job Role | Native Excel Bar | Analysis |
| 10 | Attrition by Education Field | Native Excel Column | Analysis |
| 11 | Avg Income: Active vs Attrited | Native Excel Clustered Bar | Income Analysis |

### Income & Attrition Correlation Analysis
- Statistical comparison: Mean, Median, Min, Max, Std Dev for Active vs Attrited employees
- Metrics include Monthly Income, Total Working Years, Years at Company, and Age
- Department-level income gap analysis with visual comparison chart

### Cross-Validation Review Sheet
- **10 automated integrity checks** validating data completeness and metric accuracy
- Checks: headcount, active/attrition counts, attrition rate, category counts, null detection
- All checks show green **PASS** status

---

## 🛠️ Technical Highlights

| Skill | Implementation |
|-------|---------------|
| KPI Cards | Merged-cell cards with accent-colored bottom borders |
| Conditional Formatting | DataBarRule, ColorScaleRule, CellIsRule, FormulaRule |
| Native Charts | openpyxl BarChart, PieChart with custom color palettes and axis titles |
| Freeze Panes | Frozen headers + ID column on Data sheet for scrollable navigation |
| Quality Assurance | Full pipeline: audit (0 errors), scan (0 findings), validate (passed) |

---

## 📋 How to Use

1. **Download** `HR_Analytics_Dashboard.xlsx`
2. **Open** in Microsoft Excel 2016+ or Google Sheets
3. **Navigate** sheets via bottom tabs:
   - Start with **Dashboard** for the executive overview
   - Explore **Analysis** for detailed breakdowns
   - Review **Income Analysis** for compensation insights
   - Check **Review** for data integrity validation
4. **Interact** with native Excel charts on Analysis and Income Analysis sheets (resize, filter, hover for values)
5. **Sort/Filter** the Data sheet using Excel's built-in filters

### Modifying the Dashboard
- All analysis values on the **Analysis** and **Income Analysis** sheets are computed from the source data — update the Data sheet to recalculate
- Conditional formatting rules on the Data sheet will automatically apply to new rows
- Chart data references are linked to their respective sheet tables

---

## 📊 Dataset

This project uses the **IBM HR Analytics Employee Attrition & Performance** dataset, a widely-used public dataset available on Kaggle. It contains 1,470 employee records with 35 attributes covering demographics, job characteristics, satisfaction metrics, and compensation data.

**Key data fields used:**
- Demographics: Age, Gender, Marital Status, Education, Education Field
- Job Info: Department, Job Role, Job Level, Business Travel, Over Time
- Satisfaction: Job Satisfaction, Environment Satisfaction, Relationship Satisfaction
- Compensation: Monthly Income, Daily Rate, Hourly Rate, Percent Salary Hike
- Tenure: Years At Company, Years In Current Role, Years With Curr Manager, Total Working Years

---
