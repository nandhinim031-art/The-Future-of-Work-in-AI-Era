<div align="center">

# The Future of Work in the AI Era 🤖📊
### A Data-Driven Analysis of Skills, Salaries & Hiring Trends (2023–2025)

</div>

This project explores the AI job market through exploratory data analysis (EDA), examining in-demand skills, salary trends, and hiring patterns across industries, job titles, and experience levels.

## 📌 Project Objectives

- Identify the most in-demand technical skills in AI-era job postings
- Analyze salary distributions across job titles, industries, and experience levels
- Understand hiring trends over time (2023–2025)
- Detect patterns in employment types and industry-wise job distribution
- Provide actionable insights for job seekers and employers

## 📂 Dataset Overview

| Detail | Value |
|---|---|
| Dataset Name | AI Job Market & Salary Trends |
| Time Period | 2023–2025 |
| Total Records | 2,000 |
| Total Columns | 15 |
| Missing Values | 0 |
| Duplicate Rows | 0 |

### Column Descriptions

| Column | Type | Description |
|---|---|---|
| `job_id` | int64 | Unique identifier for each job posting |
| `company_name` | object | Name of the company posting the job |
| `industry` | object | Industry sector (e.g., Tech, Healthcare, Finance) |
| `job_title` | object | Job role (e.g., Data Scientist, ML Engineer) |
| `skills_required` | object | Comma-separated list of required skills |
| `experience_level` | object | Entry, Mid, or Senior |
| `employment_type` | object | Full-time, Contract, Internship, or Remote |
| `location` | object | Geographic location of the job |
| `salary_range_usd` | object | Original salary range string (e.g., "92860-109598") |
| `posted_date` | datetime64 | Date the job was posted |
| `min_salary_usd` / `max_salary_usd` / `avg_salary_usd` | int64 | Salary figures derived from `salary_range_usd` |
| `year` / `month` / `month_year` | int32 / period | Time fields derived from `posted_date` |

## 🛠️ Tools & Libraries

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook / Google Colab

## 🔍 Project Workflow

1. **Data Loading** – Imported the raw CSV dataset
2. **Data Cleaning & Preprocessing** – Split salary ranges into min/max/avg, converted dates, checked for nulls/duplicates
3. **Descriptive Statistics** – Summarized salary, job title, industry, experience level, and employment type distributions
4. **Skill Extraction** – Parsed and counted individual skills from the `skills_required` column
5. **Data Visualization** – Built 17 charts covering salary distributions, skill demand, hiring trends over time, and industry/experience comparisons
6. **Statistical Testing** – Ran ANOVA tests to check whether salary significantly varies by experience level or industry
7. **Key Conclusions** – Synthesized findings into a final summary

## 📊 Visualizations (17 Charts)

- Distribution of average salary (histogram)
- Average salary by job title & industry (bar charts)
- Average salary by experience level (bar chart & box plot)
- Job distribution by employment type (pie chart)
- Job postings by industry & job title (bar/count plots)
- Top 15 in-demand skills (horizontal bar chart)
- Job postings over time — monthly & yearly (line/bar charts)
- Salary heatmap: industry vs. experience level
- Job count by industry & employment type (stacked bar)
- Min vs. max salary by experience level (scatter plot)
- Location uniqueness check & top-paying locations

## 💡 Key Findings

- **Volume, not salary, is the strongest signal.** Job postings roughly quadrupled from 2023 (271) to 2024 (1,006), then eased in 2025 (723) — the clearest trend in the dataset.
- **Skill and job-title demand is broad-based, not concentrated.** The top 15 skills all fall within a narrow ~51-posting band, with no single skill or title dominating.
- **Location data is synthetic.** All 2,000 postings have unique, evidently fabricated city names, ruling out meaningful location-based salary analysis.
- **Salary shows weak-to-no correlation with experience, industry, or location.** ANOVA tests returned non-significant p-values, suggesting salary was likely assigned independently of these factors — a sign of synthetic/randomly generated data rather than a real-world labor market. This makes the "no significant variation" finding itself a noteworthy result, rather than an overstated claim that experience or industry drives pay.

## 📁 Repository Structure

```
├── Main_Project.ipynb        # Full analysis notebook (EDA + visualizations)
├── ai_job_market.csv          # Dataset (2,000 rows × 15 columns)
├── README.md                  # Project documentation
```

## 🚀 How to Run

1. Clone the repository
2. Install dependencies: `pip install pandas numpy matplotlib seaborn`
3. Open `Main_Project.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab
4. Run all cells in order

## ✍️ Author

Nandhini# The-Future-of-Work-in-AI-Era
Main project -The Future of Work in AI Era
