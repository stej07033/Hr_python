# 📊 HR Employee Attrition Analysis | Python

<p align="center">
  <img src="https://img.shields.io/badge/Python-Analysis-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-Data%20Cleaning-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/NumPy-Analytics-013243?style=for-the-badge&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/Matplotlib-Visualization-11557C?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Seaborn-Statistics-4C72B0?style=for-the-badge" />
</p>

<p align="center">
  <b>Turning HR Data into Meaningful Workforce Insights</b>
  <br/>
  An end-to-end exploratory data analysis project to understand employee attrition, workforce trends, and potential employee retention challenges using Python.
</p>

---

## 📌 Project Overview

Employee attrition is an important challenge for organizations because employee turnover can affect productivity, recruitment costs, and workforce stability.

This project analyzes HR employee data using Python to identify patterns in employee attrition across departments, job roles, age groups, salary levels, job satisfaction, and overtime.

The analysis uses **Pandas, NumPy, Matplotlib, and Seaborn** to clean data, perform exploratory data analysis (EDA), calculate attrition rates, and visualize findings.

## 🎯 Project Objectives

- Analyze overall employee attrition and retention.
- Identify departments with higher attrition rates.
- Understand the relationship between overtime and employee turnover.
- Compare the age and monthly income of employees who left and stayed.
- Examine attrition patterns across job roles and satisfaction levels.
- Explore relationships between numerical HR variables.
- Generate a summary report to support data-driven HR decisions.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Data analysis and scripting |
| Pandas | Data loading, cleaning, grouping, and aggregation |
| NumPy | Numerical calculations and conditional analysis |
| Matplotlib | Data visualization |
| Seaborn | Statistical charts and heatmaps |
| Jupyter Notebook | Interactive analysis and reporting |
| CSV | Source dataset format |

## 📂 Dataset Information

The project uses an HR employee dataset containing **1,470 employee records and 44 columns**.

The dataset includes information about:

- Employee demographics: age, gender, and marital status.
- Employment details: department, job role, and business travel.
- Compensation: monthly income and salary hike.
- Job experience: total working years and years at the company.
- Employee satisfaction: job satisfaction, environment satisfaction, and work-life balance.
- Attrition: whether an employee left the organization.

**Target variable:** `Attrition`

- `Yes` — employee left the organization.
- `No` — employee stayed with the organization.

## 🔍 Project Workflow

1. **Data Loading** — Imported the HR dataset using Pandas.
2. **Data Inspection** — Examined dataset dimensions, column names, data types, and descriptive statistics.
3. **Data Quality Checks** — Checked missing values and duplicate records.
4. **Data Cleaning** — Created a working copy, removed duplicate rows, and checked important analysis columns.
5. **Exploratory Data Analysis** — Investigated attrition by department, job role, age, salary, overtime, and job satisfaction.
6. **Statistical Analysis** — Calculated attrition rates, averages, medians, and correlations.
7. **Data Visualization** — Created bar charts, histograms, box plots, and a correlation heatmap.
8. **Final Reporting** — Generated a summary of workforce attrition and key findings.

## 📈 Key Performance Indicators

| KPI | Result |
|---|---:|
| Total Employees | 1,470 |
| Employees Who Left | 237 |
| Employees Who Stayed | 1,233 |
| Overall Attrition Rate | 16.12% |
| Employee Retention Percentage | 83.88% |

## 📊 Key Analysis & Findings

### 1. Attrition by Department

| Department | Employees | Employees Left | Attrition Rate |
|---|---:|---:|---:|
| Sales | 446 | 92 | 20.63% |
| HR | 63 | 12 | 19.05% |
| R&D | 961 | 133 | 13.84% |

**Insight:** Sales has the highest department-level attrition rate at 20.63%, followed by HR at 19.05%.

### 2. Attrition by Overtime

| Overtime | Employees | Employees Left | Attrition Rate |
|---|---:|---:|---:|
| No | 1,054 | 110 | 10.44% |
| Yes | 416 | 127 | 30.53% |

**Insight:** Employees working overtime have a substantially higher observed attrition rate than employees not working overtime. This association warrants further investigation; it does not establish that overtime alone causes attrition.

### 3. Attrition by Job Role

| Job Role | Attrition Rate |
|---|---:|
| Sales Representative | 39.76% |
| Laboratory Technician | 23.94% |
| Human Resources | 23.08% |
| Sales Executive | 17.48% |
| Research Scientist | 16.10% |
| Manufacturing Director | 6.90% |
| Healthcare Representative | 6.87% |
| Manager | 4.90% |
| Research Director | 2.50% |

**Insight:** Sales Representatives have the highest attrition rate among the listed job roles, at 39.76%. HR teams could investigate role-specific workload, compensation, career development, and employee feedback.

### 4. Attrition by Age Group

| Age Group | Employees | Employees Left | Attrition Rate |
|---|---:|---:|---:|
| Under 25 | 97 | 38 | 39.18% |
| 25–34 | 554 | 112 | 20.22% |
| 35–44 | 505 | 51 | 10.10% |
| 45–54 | 245 | 25 | 10.20% |
| 55+ | 69 | 11 | 15.94% |

**Insight:** Employees under 25 have the highest observed age-group attrition rate, at 39.18%. Early-career development, onboarding, and career progression are useful areas for further investigation.

### 5. Monthly Income Analysis

| Metric | Employees Who Stayed | Employees Who Left |
|---|---:|---:|
| Average Monthly Income | 6,832.74 | 4,787.09 |
| Median Monthly Income | 5,204 | 3,202 |

**Insight:** Employees who left had lower average and median monthly incomes than employees who stayed. Compensation may be one factor to investigate alongside job role, job level, and other employee characteristics.

*Note: The original analysis does not specify the currency or unit for monthly income.*

### 6. Job Satisfaction Analysis

| Job Satisfaction Level | Stayed | Left |
|---|---:|---:|
| 1 | 76.79% | 23.21% |
| 2 | 85.56% | 14.44% |
| 3 | 85.61% | 14.39% |
| 4 | 85.45% | 14.55% |

**Insight:** The lowest job satisfaction level has the highest attrition percentage in this analysis. HR teams can investigate employee feedback, workplace experience, and engagement opportunities.

### 7. Correlation Analysis

A correlation heatmap was created to explore relationships among selected numerical variables, including:

- Age
- Monthly Income
- Job Satisfaction
- Years at Company
- Years in Current Role
- Years with Current Manager
- Distance from Home

**Insight:** Years at Company has a positive correlation of 0.76 with Years in Current Role and 0.77 with Years with Current Manager. These relationships indicate that the variables tend to increase together, but correlation does not prove causation.

## 📉 Visualizations Created

The project includes the following visual analyses:

- Employee attrition rate by department.
- Overtime versus employee attrition.
- Age distribution by attrition status.
- Monthly income comparison using a box plot.
- Attrition distribution by job satisfaction.
- Attrition rate by job role.
- Correlation heatmap of numerical HR variables.
- Age-group attrition analysis.

## 💻 Installation & Usage

### Prerequisites

Install Python 3 and Jupyter Notebook, or use an equivalent Python notebook environment.

### 1. Clone the Repository

```bash
git clone https://github.com/stej07033/HR-DASHBOARD.git
cd HR-DASHBOARD
```

### 2. Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. Add the Dataset

Place the source CSV file in your working directory. The notebook uses this filename:

```text
HR DATA_Excel 2.csv
```

### 4. Run the Analysis

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open your Python notebook and execute the cells in order.

**Important:** Update the dataset path in the code if your CSV file is stored in a different folder.

## 📁 Suggested Repository Structure

```text
HR-DASHBOARD/
│
├── data/
│   └── cleaned_hr_data.csv
│
├── outputs/
│   └── charts/
│
├── HR_Attrition_Analysis.ipynb
├── README.md
└── requirements.txt
```

This is a suggested structure; adjust filenames and folders to match the files actually committed to your repository. Avoid uploading confidential employee information or restricted datasets.

## 💡 Business Recommendations

Based on the observed patterns, HR teams could:

- Investigate the higher attrition rates among Sales Representatives.
- Review overtime practices and employee workload.
- Explore retention initiatives for early-career employees.
- Evaluate compensation across job roles and levels.
- Collect employee feedback and investigate low job satisfaction.
- Monitor attrition rates by department and job role over time.

These recommendations are starting points for further analysis rather than proven explanations for why employees leave.

## 🚀 Skills Demonstrated

- Data Cleaning and Quality Checks
- Exploratory Data Analysis (EDA)
- Data Manipulation with Pandas
- Numerical Analysis with NumPy
- Statistical Summaries
- Data Visualization
- Correlation Analysis
- Business Insight Generation
- Analytical Reporting

## 👨‍💻 About Me

**Sai Madanapalli | Aspiring Data Analyst**

I am building my skills in data analytics by working with Python, SQL, Power BI, and Excel to transform raw data into meaningful insights and support data-driven decisions.

I enjoy exploring datasets, identifying patterns, creating visualizations, and presenting analytical findings in a clear and practical way.

## 🔗 Connect With Me

- **GitHub:** [stej07033](https://github.com/stej07033)
- **LinkedIn:** [Sai Madanapalli](https://www.linkedin.com/in/madanapalli-sai-19b835389/)

---

<p align="center">
  <b>Thanks for visiting my project!</b>
  <br/>
  If you find this project useful, consider giving the repository a ⭐.
</p>
