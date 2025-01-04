
# Attrition Analytics Dashboard
![Main_Dashboard](https://github.com/user-attachments/assets/b7f09906-32d4-4883-bffe-3dd3082661e9)

### Project Overview

This Power BI project focuses on employee attrition analytics. The dashboard provides insights into employee attrition patterns by analyzing factors such as job roles, salary slabs, job satisfaction, tenurity and age groups. This helps HR teams understand attrition trends and make better decisions and reduce employee attrition.

### Dataset Information

The dataset used in this project includes employee details such as age, job role, salary, education, and job satisfaction. Please refer to the dataset file in the repository for the complete list of columns.

### Data Cleaning
During the data cleaning process, the following steps were performed to ensure data quality:
- Removed duplicate records to avoid repetition.
- Eliminated blank or missing values and replaced by 0.
- Standardized data formats for consistency.


### Custom Columns and Measures Added

Attrition Count Column
- Attrition_Count= IF(HR_Analytics[Attrition]="yes",1,0)
  
Attrition Rate Measure
- Attrition_Rate = SUM(HR_Analytics[Attrition_Count])/SUM(HR_Analytics[EmployeeCount])
  
Average Age Measure
- AvgAge = AVERAGE(HR_Analytics[Age])



### Key Insights

- Job Roles: Sales Executives and Laboratory Technicians have the highest attrition.

![Job_Role](https://github.com/user-attachments/assets/a7bf7a2e-7dfc-4b7c-b455-78ea5a69a099)

- Salary: Employees earning upto 5k have the highest attrition count.

![Salary](https://github.com/user-attachments/assets/57f9a6bb-9c9c-408e-9570-568436dd15b6)

- Age: The age group 26-35 experiences the most attrition.

![Age](https://github.com/user-attachments/assets/15f26daf-f9a0-4cfb-838b-3ac477dc2903)

- Gender: Male employees show higher attrition rates than female employees.

![Gender](https://github.com/user-attachments/assets/f6ca8d23-eabf-4c74-9435-1ff99e35c736)

- Tenurity: Shows highest attrition rate on the first of year in the company.

![Tenure](https://github.com/user-attachments/assets/fea03ae6-b17b-40a7-8f38-c774e7a185b4)

- Job satisfaction: Shows that on a scale of 1 to 4, the highest attrition is at level 3, where most employees are single and married.

![Job_Satisfaction](https://github.com/user-attachments/assets/5391c027-0c6e-40ec-a3cc-86e2efd0d891)

### Tools Used

Power BI Desktop

Microsoft Excel/CSV for Data Handling

### Project Files

- Dataset/ – Contains the dataset file.

- Screenshots/ – Contains images of the dashboard and charts.

- PowerBI_Report.pbix – The Power BI report file.

- README.md – This file explaining the project.

### How to Use This Project

1. Download or clone this repository.

2. Open the PowerBI_Report.pbix file using Power BI Desktop.

3. Use the filters to explore the dashboard and gain insights.

### Requirements

- Power BI Desktop (latest version)

- Microsoft Excel (for reviewing the dataset if needed)

### Contributing

Contributions are welcome, To contribute:

- Fork this repository.

- Create a new branch for your changes.

- Submit a pull request for review.

### License

This project is open-source and licensed under the MIT License.
