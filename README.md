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
- Score distributions across subjects
- Demographic comparisons (gender, race/ethnicity)
- Impact analysis (test prep, lunch type, parental education)
- Correlation heatmaps and regression plots

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
