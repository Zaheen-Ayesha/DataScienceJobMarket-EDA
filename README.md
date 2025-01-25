## Project Title
#### Data Science Job Market Analysis using EDA

This project provides insights into the data science job market using exploratory data analysis techniques. The analysis uncovers key trends in job titles, salaries, skills, and industry characteristics, enabling stakeholders to make informed decisions about career paths, hiring strategies, and competitive benchmarking. The size of the dataset is 12079 rows x 20 Columns. Each row in dataset contains information about job listings such as job title,company name,skill requirement etc.

### Objective
The primary objective of this project is to analyze the landscape of data science job roles by examining:
1. Salary distributions across job titles and industries.
2. Key skills required for data science roles.
3. The relationship between company attributes (e.g., size, revenue) and salaries.
4. Insights into educational qualifications and experience requirements.

### Steps Followed
#### 1. Data Loading and Cleaning:
- Imported the dataset (cleaned3.csv) into a Pandas DataFrame.
- Inspected the structure of the data, including columns like title_normalized, pay_percentile50, skill, and years_of_experience.
#### 2. Exploratory Data Analysis:
##### 1. Objective: Identify the job titles with the highest median salaries.
###### - Code Summary:

- The dataset was grouped by title_normalized to calculate the median salary (pay_percentile50) for each job title.
- The top 20 titles were extracted and visualized using a horizontal bar chart.
- A viridis color palette was applied for a gradient effect, and the y-axis was inverted for better readability.
###### - Insights:

- Titles such as "Senior Data Scientist" and "Machine Learning Engineer" dominate the top-paying jobs list.
