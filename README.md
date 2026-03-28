# Project Background & Overview
High employee turnover is expensive and disruptive for any company. This project analyzes the workforce data of 1,470 employees to understand why people are leaving the organization. By looking at attrition (employees leaving) across departments, age groups, and education levels, HR leadership can create better strategies to keep their top talent and improve job satisfaction.

**Key Business Questions:**
* Which department and education field are experiencing the highest number of employees leaving?
* Is attrition higher among a specific age group or gender?
* Does a low job satisfaction rating in specific roles (like Sales or Lab Techs) directly lead to higher turnover?

# Data Structure Overview
The data tracks individual employee profiles and their current status within the company.

* **Source:** Kaggle Public Dataset
* **Employee Profile:** Age, Gender, Education Field, and Education Level.
* **Employment Details:** Job Role, Department, and Active/Inactive status.
* **Sentiment Data:** Job Satisfaction Ratings (Scale of 1–4).

**Entity Relationship Diagram (ERD):**

![Data Model](images/hr.datamodel.png)

# Executive Summary
The organization currently has 1,470 employees with an overall Attrition Rate of 16.12% (237 people have left). The R&D department accounts for over half of all attrition (56.12%). Most employees who leave are in the 25–34 age bracket, and a significant number come from a Life Sciences education background. While the average age is 37, the "Under 25" and "25–34" groups show the highest vulnerability to leaving.

**High-Level Metrics**
* **Overall Employees**: 1,470
* **Attrition**: 237
* **Attrition Rate**: 16.12%
* **Active Employees**: 1,233
* **Average Age**: 37

![Dashboard Overview](images/consolidatedview.png)

# Insights Deep Dive
### Volume Analysis
* Sunday is consistently the busiest day of the week (**1,589 total patients**).
* The most dangerous "overload" periods occur between **00:00 and 04:00 on Mondays and Sundays**, where volume is consistently at its highest.

![Dashboard Overview](images/volumeanalysis.png)

### Demographic Equilibrium
  * Unlike the April-only view, the consolidated data shows that the **20-29** and **30-39** age groups are almost identical in volume (~1,200 each). This suggests the ER is a primary care source for young adults in this category.
![Dashboard Overview](images/demographic.png)

### Referral Source Impact
* While "None" (Walk-ins) is the largest group (**5.4K**), General Practice remains the most critical professional partner (**1.8K**).
  
![Dashboard Overview](images/referral.png)

### Monthly Story (April 2023 Deep Dive)
* When we filter down to April 2023, we see a "snapshot" of these problems. In April, the satisfaction was slightly higher (**5.30**) compared to the long-term average (**4.99**).
* This suggests that as the year progressed, patient satisfaction actually **decreased**, highlighting an urgent need for service intervention.


# Recommendations
* **Resource Scaling**: Implement a permanent "Weekend Night Shift" increase. The consolidated data proves that Sunday/Monday early mornings are a permanent trend, not a fluke.
* **Patient Experience Program**: Since the satisfaction score is trending downward (currently 4.99), the hospital should launch a "Fast-Track" program for low-acuity patients (the 50% not admitted) to get them out of the ER faster.
* **Partner Expansion**: Since General Practice sends so many patients, create a "Priority Triage" for GP-referred patients to reward the use of professional referral channels and reduce walk-in congestion.
