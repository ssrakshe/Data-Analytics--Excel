![image](https://github.com/user-attachments/assets/b1ca1a5a-ba1a-4c8d-8c0c-fc54ccd02d1b)### Project 2 Analysis
# Introduction
As a former job seeker, I’ve always been surprised by the lack of data exploring the most optimal jobs and skills in the data science market. I set out to understand what skills top employers request and how to land more pay.

# Questions to Analyze
To understand the data science job market, I asked the following:

Do more skills get you better pay?
What’s the salary for data jobs in different regions?
What are the top skills of data professionals?
What’s the pay for the top 10 skills?
Excel Skills Used

# The following Excel skills were utilized for analysis:

📊 Pivot Tables
📈 Pivot Charts
🧮 DAX (Data Analysis Expressions)
🔍 Power Query
💪 Power Pivot
Data Jobs Dataset
The dataset used for this project contains real-world data science job information from 2023. The dataset is available via my Excel course, which provides a foundation for analyzing data using Excel.

# It includes detailed information on:

👨‍💼 Job titles
💰 Salaries
📍 Locations
🛠️ Skills

# 1️⃣ Do more skills get you better pay?

🔍 Skill: Power Query (ETL)

# 📥 Extract
I first used Power Query to extract the original data (data_salary_all.xlsx) and create two queries:
🗃️ First one with all the data jobs information.
🔧 The second listing the skills for each job ID.
# 🔄 Transform
Then, I transformed each query by changing column types, removing unnecessary columns, cleaning text to eliminate specific words, and trimming excess whitespace.
📊 data_jobs_all
![](https://github.com/ssrakshe/Data-Analytics--Excel/blob/2f5726d378d943b3f8c7b7917dffe40d9ad52490/Project%202%20Dashboard/11.png)

# 🔗 Load
Finally, I loaded both transformed queries into the workbook, setting the foundation for my subsequent analysis.
📊 data_jobs_all
![](https://github.com/ssrakshe/Data-Analytics--Excel/blob/0c31d2cde388aa9631f0a25ca95c55af26b16bad/Project%202%20Dashboard/12.png)

# 📊 Analysis
💡 Insights
📈 There is a positive correlation between the number of skills requested in job postings and the median salary, particularly in roles like Senior Data Engineer and Data Scientist.

💼 Roles that require fewer skills, like Business Analyst, tend to offer lower salaries, suggesting that more specialized skill sets command higher market value.

![](https://github.com/ssrakshe/Data-Analytics--Excel/blob/e8c4371c3c5e1696d22d984695c7ca193df1ab5b/Project%202%20Dashboard/2_Project_Analysis_Chart1.png)


🤔 So What
This trend emphasizes the value of acquiring multiple relevant skills, particularly for individuals aiming for higher-paying roles.

# 2️⃣ What’s the salary for data jobs in different regions?
🧮 Skills: PivotTables & DAX
# 📈Pivot Table
🔢 I created a PivotTable using the Data Model I created with Power Pivot.
📊 I moved the job_title_short to the rows area and salary_year_avg into the values area.
🧮 Then I added new measure to calculate the median salary for United States jobs.
=CALCULATE(
    MEDIAN(data_jobs_all[salary_year_avg]),
    data_jobs_all[job_country] = "United States")
# 🧮 DAX
To calculate the median year salary I used DAX.

Median Salary := MEDIAN(data_jobs_all[salary_year_avg])
📊 Analysis
💡 Insights
💼 Job roles like Senior Data Engineer and Data Scientist command higher median salaries both in the US and internationally, showcasing the global demand for high-level data expertise.

💰 The salary disparity between US and Non-US roles is particularly notable in high-tech jobs, which might be influenced by the concentration of tech industries in the US.

![](https://github.com/ssrakshe/Data-Analytics--Excel/blob/e47e9872fd176bf487a5fc91029d7413e849756f/Project%202%20Dashboard/13.png)

🤔 So What
These salary insights are important for planning and salary negotiations, helping professionals and companies align their offers with market standards while considering geographical variations.

# 3️⃣ What are the top skills of data professionals?
🔧 Skill: Power Pivot
💪 Power Pivot
🔗 I created a data model by integrating the data_jobs_all and data_jobs_skills tables into one model.
🧹 Since I had already cleaned the data using Power Query; Power Pivot created a relationship between these two tables.

# 🔗 Data Model
I created a relationship between my two tables using the job_id column.
![](https://github.com/ssrakshe/Data-Analytics--Excel/blob/a8bde9860ed71f64f7981e466f737d0d7e7cbd81/Project%202%20Dashboard/14.png)


# 📊Analysis
💡Insights
💻 SQL and Python dominate as top skills in data-related jobs, reflecting their foundational role in data processing and analysis.

☁️ Emerging technologies like AWS and Azure also show significant presence, underlining the industry's shift towards cloud services and big data technologies.

![](https://github.com/ssrakshe/Data-Analytics--Excel/blob/67a4afa6adf09ea239804c7c2aa178f054448b1c/Project%202%20Dashboard/15.png)


🤔So What
Understanding prevalent skills in the industry not only helps professionals stay competitive but also guides training and educational programs to focus on the most impactful technologies.

# 4️⃣ What’s the pay of the top 10 skills?
📊 Skill: Advanced Charts (Pivot Chart)
📈 PivotChart
I created a combo PivotChart to plot median salary and skill likelihood (%) from my PivotTable.
🪙 Primary Axis: Median Salary (as a Clustered Column)
👍 Secondary Axis: Skill Likelihood (as a Line with Markers)
To customize the chart, I added a title axis title, removed the lines (skill likelihood), and changed the markers to diamonds.
📊 Analysis
💡Insights
💰 Higher median salaries are associated with skills like Python, Oracle, and SQL, suggesting their critical role in high-paying tech jobs.

📉 Skills like PowerPoint and Word have the lowest median salaries and likelihood, indicating less specialization and demand in high-salary sectors.

![](https://github.com/ssrakshe/Data-Analytics--Excel/blob/5d37793ae190e3e86c236932ad7c5e959c9349b3/Project%202%20Dashboard/16.png)

🤔So What
This chart highlights the importance of investing time in learning high-value skills like Python and SQL, which are evidently tied to higher paying roles, especially for those looking to maximize their salary in the tech industry.

# Conclusion
As a data enthusiast and former job seeker, I embarked on this Excel-based project to uncover valuable insights about the data science job market. Using a dataset I've curated from real-world job postings, I analyzed job titles, salaries, locations, and essential skills. By leveraging Excel features like Power Query, PivotTables, DAX, and charts, I discovered key correlations between multiple skills and higher salaries, particularly in Python, SQL, and cloud technologies.

I hope this project serves as a practical guide for data professionals and provides an overview of the skills needed for higher-paying roles.






