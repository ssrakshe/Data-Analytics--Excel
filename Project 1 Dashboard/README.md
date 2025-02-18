#### Excel Salary Dashboard
![Excel Dashboard](https://github.com/ssrakshe/Data-Analytics--Excel/blob/c0f0795535050075670b0d903fcc80461b227802/Project%201%20Dashboard/my%201st%20dashboard%20using%20excel.png)

# Introduction
This data jobs salary dashboard was created to help job seekers investigate salaries for their desired jobs and ensure they are being adequately compensated.

The data is from my Excel course, which provides a foundation in analyzing data using this powerful tool. The data contains detailed information on job titles, salaries, locations, and essential skills that are presented here.

# Excel Skills Used
The following Excel skills were utilized for analysis:

📉 Charts<br>
🧮 Formulas and Functions<br>
❎ Data Validation<br>

# Data Jobs Dataset
The dataset used for this project contains real-world data science job information from 2023. The dataset is available via my Excel course, which provides a foundation for analyzing data using Excel. It includes detailed information on:

👨‍💼 Job titles<br>
💰 Salaries<br>
📍 Locations<br>
🛠️ Skills<br>

# Dashboard Build
📉 Charts<br>
📊 Data Science Job Salaries - Bar Chart<br>
![](https://github.com/ssrakshe/Data-Analytics--Excel/blob/99e1587053b78172fee2dc448f22de342b47cb5a/Project%201%20Dashboard/1_Salary_Dashboard_Chart1.png)


🛠️ Excel Features: Utilized bar chart feature (with formatted salary values) and optimized layout for clarity.
🎨 Design Choice: Horizontal bar chart for visual comparison of median salaries.
📉 Data Organization: Sorted job titles by descending salary for improved readability.
💡 Insights Gained: This enables quick identification of salary trends, noting that Senior roles and Engineers are higher-paying than Analyst roles.

 
# 🗺️ Country Median Salaries - Map Chart
  ![](https://github.com/ssrakshe/Data-Analytics--Excel/blob/4922ba332f910661ab13ccd5b3b6ce315e9a4b0c/Project%201%20Dashboard/Screenshot%202025-02-17%20205703.png)


🛠️ Excel Features: Utilized Excel's map chart feature to plot median salaries globally.
🎨 Design Choice: Color-coded map to visually differentiate salary levels across regions.
📊 Data Representation: Plotted median salary for each country with available data.
👁️ Visual Enhancement: Improved readability and immediate understanding of geographic salary trends.
💡 Insights Gained: Enables quick grasp of global salary disparities and highlights high/low salary regions.


# 🧮 Formulas and Functions

💰 Median Salary by Job Titles

=MEDIAN(
IF(
    (jobs[job_title_short]=A2)*
    (jobs[job_country]=country)*
    (ISNUMBER(SEARCH(type,jobs[job_schedule_type])))*
    (jobs[salary_year_avg]<>0),
    jobs[salary_year_avg]
)
)

🔍 Multi-Criteria Filtering: Checks job title, country, schedule type, and excludes blank salaries.
📊 Array Formula: Utilizes MEDIAN() function with nested IF() statement to analyze an array.
🎯 Tailored Insights: Provides specific salary information for job titles, regions, and schedule types.
🔢 Formula Purpose: This formula populates the table below, returning the median salary based on job title, country, and type specified.
🍽️ Background Table

![](https://github.com/ssrakshe/Data-Analytics--Excel/blob/7fdde387d9baa2604a9a2106580372716e135534/Project%201%20Dashboard/Screenshot%202025-02-17%20210341.png)

📉 Dashboard Implementation
![](https://github.com/ssrakshe/Data-Analytics--Excel/blob/d58f79b22e5c24315e2ae8b27c301c2461567627/Project%201%20Dashboard/1.png)



# Conclusion<br>
I created this dashboard to showcase insights into salary trends across various data-related job titles. Utilizing data from my Excel course, this dashboard allows users to make informed decisions about their career paths. Exploring the functionalities to understand how location and job type influence salaries.
