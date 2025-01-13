# pandas01
To document the progress on SQL and pandas for Data Manipulation and Data Cleansing
In this module we would be focusing on beginner friendly panda functions and analysign the data and obtaining some insights from the csv file.

About the Data:
The "AI-Powered Job Market Insights" dataset provides a synthetic but realistic snapshot of the modern job market, particularly focusing on the role of artificial intelligence (AI) and automation across various industries. This dataset includes 500 unique job listings, each characterized by different factors like industry, company size, AI adoption level, automation risk, required skills, and job growth projections. It is designed to be a valuable resource for researchers, data scientists, and policymakers exploring the impact of AI on employment, job market trends, and the future of work.

Columns:
Job_Title	- object
Industry	- object
Company_Size	- object
Location	- object
AI_Adoption_Level - object
Automation_Risk - object
Required_Skills - 	object
Salary_USD	- float64
Remote_Friendly	- object
Job_Growth_Projection	- object

Rows: There are around 500 rows of data.

1. Removing the Rows that have null values since they would not be of greater use in teh analysis. Hence, removing the rows. 
2. Observation 1: Get all the rows where the better AI adaptation level is positively affecting the job growth prediction 
       Analysis: For this scenario I am considering the rows where Job_Growth_Projection is equal to 'Growth' and 'Stable'
                 Also, the AI_Adoption_Level can be 'Medium' or 'High' . 
3. Observation 2: Get all the rows based on indsutry and the Job titles involved with the industry and the skills required for each job
      Analysis: For this scenario I will be grouping all the rows based on the Industry and Jobs and then get the skills assigned to each job
4. Observation 3: Company size impacting the adoption of remote work and salaries
       Analysis: For this scenario I will be grouping the rows based on the Company size and find the mean salary for each size and the number
       of remote friendly roles available for each company size
5. Observation 4: What is the relationship between AI adoption level, company size, and job growth projections
       Analysis: For this scenario I would be grouping the rows based on AI adoption level, company size, job growth projections
6. Observation 5: Which industries and job titles are the most remote-friendly, and do they offer competitive salaries
       Analysis: I am going to get the rows based on the remote friendly nature of the role. I would also find the mean/Average of the Salaries that belong
       to a specific Job and Industry. 
   


