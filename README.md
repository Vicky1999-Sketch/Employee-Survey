# Employee-Survey-Response

![ChatGPT Image Apr 8, 2025, 07_02_45 PM](https://github.com/user-attachments/assets/795d8b29-204f-4b9e-be05-581032f17ac0)

## **Introduction**
The Employee Survey Responses dataset contains actual responses from an employee engagement survey conducted by **Pierce County, WA**, completed voluntarily by government employees.

## **Data Description**
This dataset consists of a single table:
- **HR Survey Response Table**  
  - **Columns**: 10 [Response ID, Status, Department, Director, Manager, Supervisor, Staff, Question, Response, Response Text]  
  - **Rows**: 14,725

![ESR Raw](https://github.com/user-attachments/assets/7ba45203-9994-448c-8bba-9c76bef4b745)

## **Problem Statement**
**1.** Which survey questions did respondents agree or disagree with most?  
**2.** Do you see any patterns or trends by department or role?  
**3.** As an employer, what steps might you take to improve employee satisfaction based on the survey results?
## **Methodology**
Power BI was used for data cleaning, modeling, analysis, and visualization.
## **Data Transformation / Cleaning**
1. Removed duplicate Response IDs — records reduced from 14,725 to 14,710.  
2. Changed data types and binary values (e.g., 0 for non-director, 1 for director) for better interpretation.  
3. Fixed a typo in the 7th survey question by replacing '&' with 'and'.  
4. Identified minor missing values (less than 1%) in two columns — left unchanged as they didn't affect the analysis.
## **DAX Measures**
- Count of "Agree"  
- Count of "Disagree"  
- Count of "Strongly Agree"  
- Count of "Strongly Disagree"  
- Sum of "Agree"  
- Sum of "Disagree"  
- Count of Questions  
- Count of Departments  
- Count of Response IDs
## **Findings / Insights**
### **1. Survey Questions Respondents Agreed/Disagreed With the Most**

![ESR ADQ](https://github.com/user-attachments/assets/941592e3-9cc2-48ba-97e0-287ee18574fd)

- **Most Agreed With**:  
  *“I know what is expected of me at work”* — 1,341 of 1,471 responses were in agreement.
- **Most Disagreed With**:  
  *“I have a best friend at work”* — 606 of 1,471 responses were in disagreement.
### **2. Patterns and Trends by Department or Role** 
**I. By Department**

![ESR TBD 1](https://github.com/user-attachments/assets/aa976b07-37ca-4006-9174-ec23eabcf099)

**Findings**
- Out of 21 departments, *Planning and Public Works* had the highest number of responses (4,700), while the *Family Justice Center* had the least (40).
- Overall, most departments showed more agreement than disagreement.
- Specific question-based disagreements (notably from the **Sheriff's Department**): 
  - *“In the last seven days, I have received recognition or praise for doing good work”*: 125 disagreed, 47 agreed in Sheriff's department.
  - *“I have a best friend at work”*: Even though majority (about half) of the other departments disagreed, the Sheriff's department had more agreeing (86) than disagreeing (78).
  - *“This last year, I have had opportunities to learn and grow”*: Mostly disagreed in Sheriff's department.
  - *“My supervisor holds employees accountable for performance”*: Mostly disagreed on Sheriff's department.
  - *“Overall, I am satisfied with my job”*: Mostly disagreed in Sheriff's department.
**Insight** 
The **Sheriff's Department** appears to have significantly lower employee satisfaction.

**II. By Role**

Non-Supervisors vs Supervisors                      | Non-Director vs Director
:--------------------------------------------------:|:------------------------------------------------------:
![ESR SS](https://github.com/user-attachments/assets/ce5a242d-ca43-4ac8-8f25-c635a182e456)|![ESR DD](https://github.com/user-attachments/assets/3bf523c8-12d0-4219-a973-66c0e08edfe5)

Non-Managers vs Managers                            | Non-Staff vs Staff
:--------------------------------------------------:|:------------------------------------------------------:
![ESR MM](https://github.com/user-attachments/assets/157fd182-1d69-46a9-bc83-d95ed183d69e)|![ESR NSS](https://github.com/user-attachments/assets/2737684f-6ca5-4443-ae47-cefb3bc049f5)

**Findings**
- Most responses came from:
  - Non-supervisors: 88.72%  
  - Non-directors: 98.84%  
  - Non-managers: 92.73%  
  - Non-staff: 91.5%
 ### **3. Steps to Improve Employee Satisfaction**
**Insights**:
- **Focus on the Sheriff's Department**: Address their specific issues.
- **Recognition & Appreciation**: Many employees feel underappreciated.
- **Professional Development**: Enhance learning and growth opportunities.
- **Leadership Accountability**: Improve supervisor-employee accountability.
### **Bonus question: Number of people that completed the form.

![ESR CI](https://github.com/user-attachments/assets/4acd925d-b09b-448d-81de-722ece8508d5)

**Findings**
99.08% of employees completed the form (14,575 of 14,710). This indicates high engagement/ participation of employees
## **Recommendations**
1. Prioritize concerns from the **Sheriff's Department**.
2. Strengthen **employee recognition** efforts.
3. Provide **career development opportunities**.
4. Encourage **clear communication** and **accountability** from supervisors.
5. Boost **overall job satisfaction** through department-specific strategies.
## Conclusion
While most employees understand their responsibilities and express general job satisfaction, there are areas that need attention—particularly in the Sheriff's department, where dissatisfaction is more pronounced. Key concerns include lack of recognition, limited growth opportunities, and accountability issues. Addressing these gaps through targeted strategies can significantly enhance overall employee satisfaction, retention, and performance.
## Dashboard
![ESR DB](https://github.com/user-attachments/assets/770d34d9-b7c3-42ae-9cbf-64262323d60b)




 
    









