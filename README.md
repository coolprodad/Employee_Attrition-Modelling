The dataset taken appears to be related to employee information in IBM company. Here's a brief description of what each column seems to represent:<br>

**Age:** The age of the employee. <br>
**Attrition:** Whether the employee has left the company or not (Yes/No).<br>
**BusinessTravel:** How often the employee travels for business (Non-Travel, Travel_Rarely, Travel_Frequently).<br>
**DailyRate:** The daily rate of the employee.<br>
**Department:** The department where the employee works (Sales, Research & Development, etc).<br>
**DistanceFromHome:** The distance from work to home.<br>
**Education:** The education level of the employee.<br>
**EducationField:** Field of study of the employee (Life Sciences, Medical, Other, etc).<br>
**EmployeeCount:** Count of employees. (This column seems to be constant at 1 and may not provide any useful information).<br>
**EmployeeNumber:** The number assigned to the employee.<br>
**EnvironmentSatisfaction:** Rating of the employee's environment satisfaction.<br>
**Gender:** The gender of the employee (Male/Female).<br>
**HourlyRate:** The hourly rate of the employee.<br>
**JobInvolvement:** Rating of the employee's job involvement.<br>
**JobLevel:** The level of the employee's job.<br>
**JobRole:** The role of the employee in the company (Sales Executive, Research Scientist, Laboratory Technician, etc).<br>
**JobSatisfaction:** Rating of the employee's job satisfaction.<br>
**MaritalStatus:** The marital status of the employee (Single, Married, Divorced).<br>
**MonthlyIncome:** The monthly income of the employee.<br>
**MonthlyRate:** The monthly rate of the employee.<br>
**NumCompaniesWorked**:The number of companies the employee worked at.<br>
**Over18:** Whether the employee is over 18 years old or not (Y/N).<br>
**OverTime:** Whether the employee works overtime or not (Yes/No).<br>
**PercentSalaryHike:** The percentage of the employee's salary hike.<br>
**PerformanceRating:** Rating of the employee's performance.<br>
**RelationshipSatisfaction:** Rating of the employee's relationship satisfaction.<br>
**StandardHours:** The standard number of hours the employee works. (This column seems to be constant at 80 and may not provide any useful information).<br>
**StockOptionLevel:** The level of the employee's stock option.<br>
**TotalWorkingYears:** The total number of years the employee has worked.<br>
**TrainingTimesLastYear:** The number of times the employee had training last year.<br>
**WorkLifeBalance:** Rating of the employee's work-life balance.<br>
**YearsAtCompany:** The number of years the employee has been at the company.<br>
**YearsInCurrentRole:** The number of years the employee has been in their current role.<br>
**YearsSinceLastPromotion:** The number of years since the employee's last promotion.<br>
**YearsWithCurrManager:** The number of years the employee has been with their current manager.<br>

<br>This dataset could be useful for understanding factors that contribute to **employee attrition**, factors that influence job satisfaction, or the effect of different variables on the monthly income of employees, among other things. <br>

<br>In this balancing of the target variable is done after finding the outliers and handling them using Windsorised outlier handling method then correlation of the data is been seen after that the train test split has performed where 2 models were initially developed i.e., **Logistic Regression and Decision Tree** and found that scaling of data is required before building any forcasting model for the data so **Standard Scalar** and **SMOTE** then the various models are performed like **LogisticRegression**, **DecisionTree**, **RandomForest**, **AdaBoost**, **Bagging**, **XGBC** and found that **XGBC** perform better for the IBM data set thats been considered.<br>

<img width="1055" alt="Screenshot 2023-08-02 at 2 39 35 PM" src="https://github.com/coolprodad/Sem-3/assets/109568266/857108d0-9d7f-4db2-a32b-332b71063265"> <br>

<br>From the box plot comparison diagram, we can see that Random Forest and XGBC are better models amongst all of the models. But when we observe train and test scores of Random Forest and XGBC, we can see that XGBC model is performing better on both train and test data. So we are finalizing best model as XGBC model.



