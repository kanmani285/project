**LinkedIn Job Trend Analysis**
**Objective**
The objective of this project is to scrape LinkedIn job postings, analyze skill demand trends across different cities and roles, and generate insights using data visualizations. This analysis will help understand the demand for various job skills and guide recommendations based on geographic locations and job roles.

**Tools and Technologies**
Python (Libraries: BeautifulSoup, Pandas, Matplotlib, Seaborn)

Excel (For dataset storage and export)

Google Colab (For running the code and analysis)

**Project Phases**
**Phase 1: Data Cleaning and Preprocessing**
Dataset: The dataset (linkedin_job_posts_insights.xlsx) contains job postings scraped from LinkedIn. It includes columns such as job title, company name, location, hiring status, date, seniority level, job function, employment type, and industry.

Steps:

Imported libraries and loaded the dataset into a Pandas DataFrame.

Cleaned text columns to remove unnecessary spaces and newline characters.

Dropped duplicate entries and handled missing values in the critical columns (job_title, location).

Split location data into separate columns for city, state, and country.

**Phase 2: Skill Trends by City – Heatmap**
Skill Extraction: A predefined list of skills (e.g., Python, SQL, Data Science, etc.) was used to extract skills mentioned in the job titles.

Steps:

Skills were extracted from job titles using keyword matching.

The data was exploded, so each skill appeared on a separate row with corresponding cities.

A heatmap was generated to visualize the demand for top 10 skills across different cities.

**Phase 3: Skill vs Role Matrix**
Role Extraction: Common job roles (e.g., Data Analyst, Data Scientist, Machine Learning Engineer) were mapped from job titles.

Steps:

Extracted job roles from job titles.

Created a matrix to compare the frequency of skills within each job role.

A heatmap visualizing the skill frequency by job role was generated.

**Phase 4: Job Demand Recommendation System**
Skill-Based Recommendations: A recommendation system was created to suggest top cities and job roles based on a given skill.

Steps:

Provided functionality to recommend the top cities for specific skills.

Also recommended the top job roles for a given skill based on the data.

**Files in this Repository**
LinkedIn_Job_Trend_Analysis.ipynb: The Jupyter notebook containing all the code and analysis steps.

cleaned_linkedin_jobs.xlsx: The cleaned dataset after preprocessing.

linkedin_job_posts_insights.xlsx: The original dataset containing raw job posting data from LinkedIn.
