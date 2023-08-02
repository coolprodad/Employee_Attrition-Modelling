The dataset taken appears to be related to employee information in IBM company. Here's a brief description of what each column seems to represent:

**Age:** The age of the employee.
**Attrition:** Whether the employee has left the company or not (Yes/No).
**BusinessTravel:** How often the employee travels for business (Non-Travel, Travel_Rarely, Travel_Frequently).
**DailyRate:** The daily rate of the employee.
**Department:** The department where the employee works (Sales, Research & Development, etc).
**DistanceFromHome:** The distance from work to home.
**Education:** The education level of the employee.
**EducationField:** Field of study of the employee (Life Sciences, Medical, Other, etc).
**EmployeeCount:** Count of employees. (This column seems to be constant at 1 and may not provide any useful information).
**EmployeeNumber:** The number assigned to the employee.
**EnvironmentSatisfaction:** Rating of the employee's environment satisfaction.
**Gender:** The gender of the employee (Male/Female).
**HourlyRate:** The hourly rate of the employee.
**JobInvolvement:** Rating of the employee's job involvement.
**JobLevel:** The level of the employee's job.
**JobRole:** The role of the employee in the company (Sales Executive, Research Scientist, Laboratory Technician, etc).
**JobSatisfaction:** Rating of the employee's job satisfaction.
**MaritalStatus:** The marital status of the employee (Single, Married, Divorced).
**MonthlyIncome:** The monthly income of the employee.
**MonthlyRate:** The monthly rate of the employee.
**NumCompaniesWorked:**The number of companies the employee worked at.
**Over18:** Whether the employee is over 18 years old or not (Y/N).
**OverTime:** Whether the employee works overtime or not (Yes/No).
**PercentSalaryHike:** The percentage of the employee's salary hike.
**PerformanceRating:** Rating of the employee's performance.
**RelationshipSatisfaction:** Rating of the employee's relationship satisfaction.
**StandardHours:** The standard number of hours the employee works. (This column seems to be constant at 80 and may not provide any useful information).
**StockOptionLevel:** The level of the employee's stock option.
**TotalWorkingYears:** The total number of years the employee has worked.
**TrainingTimesLastYear:** The number of times the employee had training last year.
**WorkLifeBalance:** Rating of the employee's work-life balance.
**YearsAtCompany:** The number of years the employee has been at the company.
**YearsInCurrentRole:** The number of years the employee has been in their current role.
**YearsSinceLastPromotion:** The number of years since the employee's last promotion.
**YearsWithCurrManager:** The number of years the employee has been with their current manager.

This dataset could be useful for understanding factors that contribute to **employee attrition**, factors that influence job satisfaction, or the effect of different variables on the monthly income of employees, among other things. 

In this balancing of the target variable is done after finding the outliers and handling them using Windsorised outlier handling method then correlation of the data is been seen after that the train test split has performed where 2 models were initially developed i.e., **Logistic Regression and Decision Tree** and found that scaling of data is required before building any forcasting model for the data so **Standard Scalar** and **SMOTE** then the various models are performed like **LogisticRegression**, **DecisionTree**, **RandomForest**, **AdaBoost**, **Bagging**, **XGBC** and found that **XGBC** perform better for the IBM data set thats been considered.

<img width="1055" alt="Screenshot 2023-08-02 at 2 39 35 PM" src="https://github.com/coolprodad/Sem-3/assets/109568266/857108d0-9d7f-4db2-a32b-332b71063265">

From the box plot comparison diagram, we can see that Random Forest and XGBC are better models amongst all of the models. But when we observe train and test scores of Random Forest and XGBC, we can see that XGBC model is performing better on both train and test data. So we are finalizing best model as XGBC model.



