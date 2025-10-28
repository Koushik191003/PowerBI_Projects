# Employees Attrition Analysis
## Objective
The main objective of this project is to analyze employee attrition patterns to identify key factors influencing workforce turnover and to support management in improving employee retention strategies.
## Project Highlights
This project focuses on studying employee turnover across different departments, job roles, and demographic segments such as age, gender, education field, and job satisfaction. The dataset provides detailed information about employees, helping to identify areas where attrition is most prevalent. The dashboard highlights key metrics such as overall attrition rate, average employee age, and department-wise turnover, providing a clear picture of workforce stability and satisfaction levels.
## Dashboard Visualization
<img width="1178" height="662" alt="DASHBOARD" src="https://github.com/user-attachments/assets/03191335-5d4d-4729-ad3a-45002d632338" />

## Dashboard Insights
### 1. Overall Attrition KPIs
This section provides an overview of the organization’s employee structure, showing total employees, attrition percentage, and average age. It helps in understanding the overall workforce condition and identifying whether turnover rates are within a manageable range.

### 2. Department-wise Attrition Chart
This visualization highlights the departments that experience higher employee turnover. It helps management identify which departments need immediate focus to improve employee satisfaction and reduce quitting rates.

### 3. Gender and Age Distribution Chart
This chart represents attrition patterns based on gender and age. It reveals which demographic groups are more likely to leave, helping in designing targeted retention programs for specific employee segments.

### 4. Education Field Chart
This chart provides insights into how employees from different educational backgrounds are distributed across attrition trends. It helps HR teams understand whether employees from certain academic streams are facing career alignment issues within the organization.

### 5. Job Satisfaction Overview
This visualization displays the overall job satisfaction level across employees. It indicates whether workplace culture, recognition, or growth opportunities are affecting employee morale and retention.
## DAX Formulas Used
- Average Age = AVERAGE(HR[Age])
- Total Employee = COUNT(HR[Employee Count])
- Percentage Attrition = DIVIDE([Employee Quit],[Total Employee],100)
- Employee Quit = CALCULATE(COUNT(HR[CF_attrition label]),KEEPFILTERS(HR[CF_attrition label]="Ex-Employees"))
- CurrentEmployee = CALCULATE(COUNT(HR[CF_attrition label]),KEEPFILTERS(HR[CF_attrition label]="Current Employees"))
## Conclusion
The analysis highlights that employee attrition is concentrated in specific departments, with HR and R&D showing the highest turnover. Younger employees, particularly males in the 25–34 age range, and those from Life Sciences and Medical backgrounds, are the most vulnerable to leaving. Job satisfaction and career growth opportunities are key factors influencing their decision to exit.To reduce attrition and enhance employee retention, the organization should:

- Identify the key reasons behind higher turnover in HR and R&D and implement targeted retention strategies.

- Provide mentorship programs, skill development, and career progression plans to retain younger staff.

- Collect continuous feedback and address concerns related to workload, recognition, and work-life balance.

- Ensure competitive compensation and growth opportunities, particularly for employees with specialized skills.

#### Applying these measures will help the organization retain critical talent, stabilize high-turnover departments, and foster a more motivated and satisfied workforce.
