![Hospital](https://viehealthcare.com/wp-content/uploads/2022/04/VIE-Healthcare-The-Role-of-A-Health-Data-Analyst-Image-of-doctor-looking-at-a-3d-representation-of-a-human-body-1024x510.jpg)

# Power_BI_Hospital_Data_Analysis
This repository contains a comprehensive Power BI dashboard project focusing on hospital data visualization. The dashboard is designed to provide insightful analytics and facilitate data-driven decision-making processes within healthcare organizations.

# Objectives
The primary objectives of this project are:

######  To create an interactive and visually appealing Power BI dashboard for hospital data analysis.
######  To demonstrate proficiency in data collection, transformation, modeling, and visualization using Power BI.
######  To showcase skills in designing and implementing end-to-end data analytics solutions.

# Project Context
In the healthcare industry, effective data analysis is crucial for optimizing operational efficiency, improving patient outcomes, and making informed decisions. This Power BI dashboard aims to offer insights into hospital operations, such as waitlist management, resource allocation, and trend analysis, to support stakeholders in their decision-making processes.


# Data Sources
The data utilized in this project comprises various hospital datasets, including inpatient and outpatient records, obtained from internal sources or simulated for demonstration purposes.

# Sample Data
## Inpatient Table
The inpatient table comprises records of patients admitted to the hospital for medical treatment or surgical procedures that necessitate an overnight stay for observation or intervention.

|       | Archive_Date   |   Specialty_HIPE | Specialty_Name   | Case_Type   | Adult_Child   | Age_Profile   | Time_Bands   |   Total |
|------:|:---------------|-----------------:|:-----------------|:------------|:--------------|:--------------|:-------------|--------:|
| 27298 | 31-07-2019     |             1800 | Orthopaedics     | Day Case    | Adult         | 16-64         | 15-18 Months |      35 |
| 21962 | 31-05-2019     |             7800 | Urology          | Day Case    | Adult         | 16-64         | 12-15 Months |       9 |
|  2062 | 31-01-2019     |             1400 | Neurosurgery     | Inpatient   | Adult         | 65+           | 15-18 Months |       5 |
| 25904 | 30-06-2019     |             7800 | Urology          | Inpatient   | Adult         | 65+           | 15-18 Months |       1 |
| 48379 | 31-12-2019     |             1902 | Paed Cardiology  | Day Case    | Child         | 16-64         | 0-3 Months   |       8 |


## Outpatient Table
The Outpatient table contains data about medical services provided to patients who do not require an overnight stay in the hospital, typically including consultations, diagnostics, and minor procedures. 

|       | Archive_Date   |   Specialty_HIPE | Speciality      | Adult_Child   | Age_Profile   | Time_Bands   |   Total |
|------:|:---------------|-----------------:|:----------------|:--------------|:--------------|:-------------|--------:|
|   917 | 31-01-2018     |             1700 | Ophthalmology   | Adult         | 65+           | 3-6 Months   |      45 |
| 38139 | 30-06-2018     |              100 | Cardiology      | Adult         | 16-64         | 0-3 Months   |     478 |
| 58052 | 30-09-2018     |             2600 | General Surgery | Adult         | 65+           | 0-3 Months   |     156 |
| 76205 | 31-12-2018     |              400 | Endocrinology   | Child         | 0-15          | 12-15 Months |       2 |
| 77733 | 31-12-2018     |             7800 | Urology         | Adult         | 65+           | 6-9 Months   |      81 |

## Speciality Mapping
Specialty mapping involves categorizing specialties into groups for easier analysis and visualization, enhancing the understanding of hospital data trends and patterns.

|    | Specialty                   | Specialty Group   |
|---:|:----------------------------|:------------------|
| 71 | Radiotherapy                | General           |
| 13 | General Surgery             | General           |
| 47 | Pain Relief                 | General           |
| 62 | Oncology                    | Cancer            |
|  3 | Child/Adolescent Psychiatry | Psychatry         

# Project Overview
## Data Transformation and Modeling
In the data transformation and modeling phase of the project, the process involves importing hospital datasets, applying data transformations using Power Query Editor, and modeling the data to create a unified dataset. This includes appending inpatient and outpatient data, creating relationships between tables, and utilizing mapping tables for categorization. Additionally, meticulous attention is paid to data integrity during the cleaning phase, ensuring consistency and accuracy by removing extraneous spaces, standardizing formats, and addressing missing or erroneous values. This prepares the data for robust analysis and visualization in the subsequent stages of the project.

## Data Visualization Blueprint
The dashboard design phase focuses on creating a summary page and a detailed granular-level page. The summary page includes key metrics, trend analysis, and top specialties, while the detailed page provides a more comprehensive view of the data. Advanced visualizations and interactive elements are utilized to enhance user experience.

## Dashboard Design and Beautification
Inspired by modern design principles, the dashboard is aesthetically enhanced using color schemes extracted from images and shapes for background design. The presenter demonstrates formatting charts, adding dynamic titles, and utilizing PowerPoint for background design.

## Interactivity and Navigation
The dashboard is made interactive with toggle buttons, slicers, and filters. Navigation between summary and detailed pages is facilitated through buttons, and drill-down features provide a deeper insight into the data. Measures are implemented to handle data visibility and messaging for user guidance.

## Sharing and Maintenance
The final phase involves sharing the dashboard with stakeholders via Power BI services, ensuring data security through row-level security (RLS), and documenting the refresh process for routine maintenance. 

# Summary Page
The summary page contains two main indicators, mean and median, for analyzing key metrics, This Page utilizes the switch function to enable users to toggle between displaying average and median values for key metrics. This provides flexibility in analyzing data and allows users to choose the most appropriate indicator based on their specific needs and preferences.

![image](https://github.com/amine-abdollah/Power_BI_Hospital_Data_Analysis/assets/103480107/ae0bfec4-651f-41a7-9048-12c83decfde5)


## Key Metrics
### Current Month Wait List
Displays the total number of patients currently on the waitlist for the current month.
### Previous Year Wait List
This shows the total waitlist count for the same month in the previous year.
## Bifurcation Chart
### Donut Chart
Illustrates the distribution of patients across outpatient, inpatient, and day-cases waiting lists.
## Age Profile Analysis
### Stacked Column Chart:
Visualizes the relationship between age profile and time band, providing insights into patient demographics.
## Top Specialties
### Grid
Highlights the top 5 specialties with their average wait lists, allowing users to toggle between average and median values.
## Monthly Trend Analysis
### Line Charts
Tracks the trend of inpatient, day cases, and outpatient categories over different months, with filters for month, case type, and specialty.

# Detailed Page
The Detailed View Page offers users a deeper dive into the data with more comprehensive visualizations and detailed insights.

![image](https://github.com/amine-abdollah/Power_BI_Hospital_Data_Analysis/assets/103480107/24c1efbb-626c-44b4-804f-5726a4a854b9)

## Filters
### Specialty
Allows users to filter data based on specialty.
### Time Band 
Filters data based on time bands.
## Matrix View
### Matrix
Provides a detailed view of the data, summarized and formatted for better readability.
# Drill Down Page
The drill-down page offers a more detailed view of the data when users interact with specific elements on the summary page. It includes additional charts and visuals to provide deeper insights into selected data points, enhancing the user's analytical capabilities, In our Cases The page provides a breakup of the total wait list by Speciality for a deeper Analysis.

![image](https://github.com/amine-abdollah/Power_BI_Hospital_Data_Analysis/assets/103480107/6f314000-554d-4cc2-9213-96c04f4de9a9)

# Conclustion
This Power BI dashboard project showcases the end-to-end process of creating a comprehensive analytics solution for hospital data, enabling stakeholders to make informed decisions and optimize operational efficiency. Through meticulous data transformation, modeling, and visualization, the project provides insights into key metrics, trends, and specialties, facilitating a deeper understanding of hospital operations. Moreover, the technical benefits of the project extend to improved data integrity, streamlined analysis processes, and enhanced visualization capabilities, empowering users to extract valuable insights efficiently.

