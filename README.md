# Texas_Superintendent_Salaries_2024-2025_Analysis-
Business Intelligence Style/ Reporting Analysis of the Superintendent Salaries for the state of Texas from 2024-2025

Overview

Data Source
• Data was sourced from data.gov which was listed through data.austintexas.gov
• Link: https://catalog.data.gov/dataset/superintendent-salary-report-by-district-for-school-year-2024-2025


Data Cleaning/Formatting
• Assigned appropriate data types to each column (e.g., Currency for pay fields, Whole Number for Enrollment) 
• Removed two columns containing only "Not Reported" values (redundant metadata)
• One row enrollment was labeled "-999"; corrected the negative
• Filled two FTE Pay values with matching Base Pay values (assumed equivalence in context)
• Removed one entry for Loving county (no active school district due to extremely low population)


Feature Engineering
• Base Pay Per Enrollment -> Base Pay Per Child
• FTE Pay Per Enrollment -> FTE Pay Per Child
• FTE Pay  Overall -> Designated Low/Medium/High Pay
• Turnover -> District <1  Designated (Single/Partial)
• FullTime/PartTime -> FTE > 1 (Full Pay/Partial)

