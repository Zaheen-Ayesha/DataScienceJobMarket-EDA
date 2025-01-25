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
![Image_Alt](https://github.com/Zaheen-Ayesha/DataScienceJobMarket-EDA/blob/fe6aada568cdc9c2b367c89c2f94215fac797c52/topjob.png)

##### 2. Objective: Highlight companies offering the highest salaries.
###### - Code Summary:
- Median salaries were computed for each company using pay_percentile50.
- A bar chart was created using Seaborn's YlOrRd palette for a warm gradient effect.
- Additional formatting included gridlines and rotated x-axis labels for readability.
###### - Insights:
- Top-tier tech companies appear prominently, indicating their competitive compensation strategies.
![Image_Alt](https://github.com/Zaheen-Ayesha/DataScienceJobMarket-EDA/blob/fe6aada568cdc9c2b367c89c2f94215fac797c52/topcomp.png)

##### 3. Objective: Explore companies offering the lowest median salaries.
###### - Code Summary:
- Similar to the highest-paying companies, the dataset was grouped by company and sorted by median salary in ascending order.
- A bar chart with the cividis palette was used for visualization.
- Labels and gridlines were customized to ensure clarity.
###### - Insights:
- Smaller or less profitable firms dominate this list, reflecting their limited budget for salaries.
![Image_Alt](https://github.com/Zaheen-Ayesha/DataScienceJobMarket-EDA/blob/fe6aada568cdc9c2b367c89c2f94215fac797c52/lowcomp.png)

##### 4. Objective: Analyze the distribution of required years of experience.
###### - Code Summary:
- A box plot was created to summarize the distribution of years_of_experience.
- The plot used a steelblue color scheme for visual appeal.
###### - Insights:
- Most roles require 2–5 years of experience, with outliers for senior-level positions demanding significantly more.
![Image_Alt](https://github.com/Zaheen-Ayesha/DataScienceJobMarket-EDA/blob/fe6aada568cdc9c2b367c89c2f94215fac797c52/exp.png)

##### 5. Objective: Highlight the most in-demand skills for data science roles.
###### - Code Summary:
- A horizontal bar chart was created using the magma palette to show the frequency of top 10 skills.
- A word cloud was generated using the WordCloud library, applying the magma colormap to match the bar chart’s theme.
###### - Insights:
- Skills like Python, SQL, and Machine Learning dominate the job market.
- The word cloud effectively complements the bar chart by emphasizing popular skills visually.
![Image_Alt](https://github.com/Zaheen-Ayesha/DataScienceJobMarket-EDA/blob/fe6aada568cdc9c2b367c89c2f94215fac797c52/skill.png)

##### 6. Objective: Examine the education levels required for data science roles.
###### - Code Summary:
- The dataset was filtered for columns representing different education levels (e.g., doctoral, master, bachelor).
- A pie chart was used to display the proportion of each education level, with colors from the Paired palette.
###### - Insights:
- Master’s degrees are most common among data professionals, followed by bachelor’s degrees.
![Image_Alt](https://github.com/Zaheen-Ayesha/DataScienceJobMarket-EDA/blob/fe6aada568cdc9c2b367c89c2f94215fac797c52/edu.png)

##### 7. Objective: Discover which industries have the most job postings.
###### - Code Summary:
- The top 10 industries were identified by the count of job listings.
- A horizontal bar chart with the YlGnBu palette was used for visualization.
###### - Insights:
- Technology and finance industries lead in job postings for data professionals.
![Image_Alt](https://github.com/Zaheen-Ayesha/DataScienceJobMarket-EDA/blob/fe6aada568cdc9c2b367c89c2f94215fac797c52/indu.png)

##### 8. Objective: Identify the sectors offering the highest median salaries.
###### - Code Summary:
- Median salaries for sectors were calculated, sorted, and visualized using a bar chart with the summer palette.
- Gridlines and rotated labels were included for clarity.
###### - Insights:
- Sectors like finance and pharmaceuticals offer the highest pay for data roles
![Image_Alt](https://github.com/Zaheen-Ayesha/DataScienceJobMarket-EDA/blob/fe6aada568cdc9c2b367c89c2f94215fac797c52/sec.png)

##### 9. Objective: Analyze how working at company headquarters affects salary.
###### - Code Summary:
- A box plot was created to compare salaries for roles at headquarters (at_heartquartes) versus non-HQ locations.
- Numerical labels were replaced with descriptive text (e.g., "At HQ" and "Not At HQ").
###### - Insights:
- Roles based at headquarters tend to have higher median salaries, possibly due to proximity to decision-makers.
![Image_Alt](https://github.com/Zaheen-Ayesha/DataScienceJobMarket-EDA/blob/fe6aada568cdc9c2b367c89c2f94215fac797c52/head.png)


