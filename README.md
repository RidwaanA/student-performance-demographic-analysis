# 🎓 Student Academic Performance & Demographic Analysis

## Project Overview
This project analyzes student performance across math, reading, and writing to uncover how demographic and socioeconomic factors influence academic outcomes.

Using Python (Pandas, Seaborn, Matplotlib), the analysis identifies performance gaps and success drivers, enabling data-driven educational strategies.

## Business Problem
Excellent Minds seeks to improve student outcomes by understanding:

- What drives high vs low academic performance
- How demographics impact results
- Which interventions are most effective

## Dataset
- 1,000 students
- 8 features including:
  `math score`, `reading score`, `writing score`, `gender`, `parental education`, `lunch`, `test preparation`
- Mix of demographic and performance data

## Tools & Technologies
- **Python** (Pandas, NumPy, Seaborn, Matplotlib)
- **Jupyter Notebook**
- **Tableau**

## Data Processing / Methodology
- Validated dataset (no missing values or duplicates)
- Performed univariate, bivariate, and multivariate analysis
- Conducted correlation and distribution analysis
- Analyzed performance across demographic and socioeconomic segments

## Key Code Highlights
```python
// Correlation between subject scores
corr = data.corr()
sns.heatmap(corr, annot=True, vmin=-1, vmax=1, fmt='.2f', cmap='Spectral');
```
```python
// Impact of test preparation
sns.lineplot(data=data, x='test preparation course', y='math score', ci=None)
plt.show()
```
```python
// Performance by parental education and gender
data.groupby(['parental level of education','gender'])['reading score'].mean()
```

## Visualization / Dashboard

**Python (Jupyter Notebook)**
- 📌 Score distributions across math, reading, and writing subjects
- 📌 Demographic comparisons across gender and race/ethnicity
<img width="378" height="382" alt="Bar chart_Gender count" src="https://github.com/user-attachments/assets/601d9160-3c76-455d-b7da-d1fcc0dbb2b6" />


- 📌 Impact analysis for test preparation course, lunch type, and parental education level
- 📌 Correlation heatmaps and regression plots across score variables
<img width="874" height="315" alt="Heat map_Numerical features1" src="https://github.com/user-attachments/assets/3dfc5c0a-f8ba-49d1-8125-abb47150f9a3" />

---

**Tableau**
- 📌 Highlight table: Student gender distribution across the dataset
- 📌 Highlight table: Average math, reading, and writing scores across gender groups
- 📌 Highlight table: Average math, reading, and writing scores across test preparation course completion status
- 📌 Scatter plot: Average reading score against math score across gender groups
- 📌 Scatter plot: Average reading score against writing score across gender groups
- 📌 Scatter plot: Average writing score against math score across gender groups
- 📌 Bar charts: Average math, reading, and writing scores across race/ethnicity groups
- 📌 Bar charts: Average math, reading, and writing scores across parental levels of education
- 📌 Bar charts: Average math, reading, and writing scores across lunch groups

[**Dashboard Overview**]
<img width="1366" height="768" alt="Screenshot (585)" src="https://github.com/user-attachments/assets/ecce27df-a579-44bb-9698-1021e856aade" />

  🔗 **[View Live Dashboard on Tableau Public](https://public.tableau.com/views/StudentAcademicPerformanceDemographicProfileAnalysis/StudentReadingScoreSummary?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)**


## Key Insights
**Academic Performance Trends**
- Students perform best in reading, followed by writing, then math
- Strong positive correlation across all subjects

**Gender-Based Performance**
- Male students perform better in math
- Female students outperform in reading and writing

**Parental Education Impact**
- Higher parental education → higher student performance
- Lowest scores from students with high school / some high school backgrounds

**Socioeconomic Influence**
- Students with standard lunch outperform those with free/reduced lunch
- Indicates strong link between socioeconomic status and performance

**Test Preparation Effectiveness**
- Students who completed test prep courses consistently outperform others across all subjects

**Demographic Trends**
- Highest-performing groups: Race/Ethnicity Groups D & E
- Lowest-performing group: Group A

## Recommendations
**For Institutions**
- Expand and potentially mandate test preparation programs
- Implement targeted academic support for low-performing demographic groups
- Introduce math-focused interventions, especially for female students
- Provide additional resources for economically disadvantaged students

**For Strategy & Policy**
- Use data-driven teaching approaches to personalize learning
- Strengthen parental engagement programs, especially for lower education backgrounds
- Leverage strengths in reading/writing to improve math outcomes

## Outcome / Impact
This analysis enables:

- ✅ Identification of performance gaps and at-risk student groups
- ✅ Development of targeted intervention strategies
- ✅ Improved academic planning and resource allocation
- ✅ Data-backed education policy decisions

## Next Steps
- Build a student performance prediction model
- Develop early-warning systems for at-risk students
- Create an interactive Tableau dashboard for educators
