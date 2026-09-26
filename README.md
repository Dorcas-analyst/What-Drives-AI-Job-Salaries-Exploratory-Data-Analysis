# What-Drives-AI-Job-Salaries-Exploratory-Data-Analysis

## Project Overview

This project analysed **15,000 AI job postings worldwide** to investigate the factors associated with AI job salaries, identify the most in-demand technical skills, and examine commonly assumed salary drivers such as education and remote work.
This was a **descriptive and exploratory data analysis project**, not a predictive machine-learning project. The analysis used Python, pandas, NumPy, Matplotlib, and Seaborn.

## Objectives
* Assess dataset quality and structure.
* Explore salary distributions.
* Analyse salary by experience level, education, company size, and remote-work arrangement.
* Identify the most frequently requested AI skills.
* Examine relationships between salary and available numeric variables.
* Identify meaningful patterns and negative findings.
* Document limitations affecting interpretation.

## Dataset
**15,000 records × 19 columns**

Key variables included:
`salary_usd`, `experience_level`, `employment_type`, `company_location`, `company_size`, `employee_residence`, `remote_ratio`, `required_skills`, `education_required`, `years_experience`, `industry`, `benefits_score`, and others.

Data quality checks found:
* **0 missing values**
* **0 duplicate rows**
The posting and application-deadline columns were converted to datetime format.

## Data Preparation
The `required_skills` column contained comma-separated skill strings. I split, cleaned, flattened, and counted individual skills to determine the most frequently requested technologies across the dataset.

## Key Findings
### Seniority and Salary
Average salary increased substantially across experience levels:
| Level     | Approx. Average Salary |
| --------- | ---------------------: |
| Entry     |                   $63K |
| Mid       |                   $88K |
| Senior    |                  $122K |
| Executive |                  $188K |
Seniority was the most consistent salary-related pattern in the dataset.

### Most Requested AI Skills
The leading skills were:
**Python → SQL → TensorFlow → Kubernetes → Scala → PyTorch**
The wider top-skills list also included cloud, infrastructure, programming, and machine-learning technologies.

### Remote Work and Salary
Salary vs. remote ratio correlation: **+0.014**
This is essentially zero, and the salary distributions across on-site, hybrid, and fully remote roles were also very similar.

### Education and Salary
Salary distributions across Associate, Bachelor, Master, and PhD requirements were broadly similar, showing little visible salary premium associated with formal education level in this dataset.

### Company Size
Large companies showed higher median salaries than medium and small companies, although the difference was considerably smaller than the seniority effect.

## Important Data Limitation
The dataset showed a perfect mapping between `years_experience` and `experience_level`, with no overlap between the experience bands.
This suggests the data may contain synthetic or algorithmically generated structure. Therefore, the findings should be treated as **directional insights about this dataset rather than definitive benchmarks for the global AI job market**.

## Skills Demonstrated
**Python · pandas · NumPy · Matplotlib · Seaborn · Exploratory Data Analysis · Data Cleaning · Data Visualisation · Statistical Analysis · Correlation Analysis · Text Parsing · Frequency Analysis · Business Insight Generation · Technical Report Writing**

## Code & Report Attribution
The base analytical code was **adapted from a public Kaggle notebook by Omar Yasser**, with modifications made for this project.
**The technical report was researched, structured, interpreted, and written independently by me**, including the analytical narrative, chart interpretation, cross-referencing of findings, limitations, and recommendations.

## Future Analysis
Potential next steps include:
* Adding `years_experience` to the correlation analysis.
* Analysing salary against benefits score visually.
* Comparing skill requirements by experience level.
* Analysing salary by industry.
* Testing predictive models to quantify how much salary variation can be explained by seniority, job title, and other factors.

## Key Takeaway
This analysis showed that **seniority was the clearest salary-related factor**, while Python emerged as the most frequently requested technical skill. Remote-work arrangement and benefits score showed virtually no linear relationship with salary, while education level showed little visible salary differentiation in this dataset.
The project demonstrates my ability to move beyond basic visualisation and perform **structured exploratory analysis, identify meaningful and negative findings, challenge assumptions, document limitations, and communicate technical findings through a detailed analytical report.**
