# Baltimore City Employee Jobs Cluster Analysis
Categorizing jobs in Baltimore city government by years worked, gross pay, and annual pay in FY2020
## Background
Based on the [finding of The Baltimore Sun](https://www.baltimoresun.com/maryland/baltimore-city/bs-md-ci-consent-decree-report-20200122-pth324df5vexxbrzyn7m6ebzwy-story.html), Baltimore city government, especially Baltimore police department, is experiencing shortages in employees and high turnover rates. Such phenomeon has caused delay in critical reforms and other essential affairs. In addition, [high turnover rates](https://www.hrdconnect.com/2019/09/10/the-impact-of-high-staff-turnover-on-company-culture/) can result in other negative consequences such as loss of valuable skills in the organization and loss of morale and trust in the teams. This analysis will focus on grouping various jobs in Baltimore city government based on years the employees worked, gross pay, and annual pay in FY2020 to further analyze strategies Baltimore city government can execute in order to retain employees and better allocate their budgets.
## Business Question
How can jobs in Baltimore city be categorized based on years worked, gross pay, and annual pay in FY 2020 and what strategies can Baltimore city government execute to encourage higher retention rate and better distribute their budgets based on this analysis?
## Open Data
The Baltimore employee salaries dataset was downloaded from [Baltimore Open Data](https://data.baltimorecity.gov/).
This [dataset](https://github.com/ireneliu0106/Baltimore-city-employee-cluster-analysis/blob/main/Baltimore_Employee_Salaries.xlsx) includes information about Baltimore city employee, including their names, agency ID, agency name, job title, hire date, gross pay, annual salary, fiscal year, etc.
## Data Analysis
Here are the [Excel file for data analysis] and the [step-by-step descriptions of Excel data analysis](https://github.com/ireneliu0106/Baltimore-city-employee-cluster-analysis/blob/main/Step-by-step%20instructions%20of%20Excel%20data%20analysis).

The dataset does not explicitly contain the data for years worked in Baltimore city government of each employee. Therefore, it was calculated by subtracting 3/18/2021 by the hire date of each employee. Pivot table was generated to find the average years worked, gross pay, and annual salary in FY2020 of employees for each job. 4 anchor nodes were used in the cluster analysis. 

### What are the characteristics of each cluster node?
<img width="888" alt="Screen Shot 2021-03-16 at 12 53 29 PM" src="https://user-images.githubusercontent.com/70459912/111348466-9df01b00-8656-11eb-80de-7d61b8f12db3.png">
<img width="1180" alt="Screen Shot 2021-03-16 at 12 54 07 PM" src="https://user-images.githubusercontent.com/70459912/111348561-b4967200-8656-11eb-9ca0-5e3f59039fe2.png">

As shown in the graph, _cluster 1 node_, which is Control System Operator, is characterized by the low years worked in Baltimore city government, lowest gross pay, and lowest annual salaries. The z scores of all three variables in for this cluster node are negative, meaning that the jobs fall in cluster 1 have years worked, gross pay, and annual salaries in FY2020 lower than the mean. 

On the other hand, _cluster 2 node_, which is F&P Benefits Analyst Superviser, has negative z scores for years worked and positive z scores for gross pay and annual salaries in FY2020. Although the gross pay and annual salary are higher than the mean, the years the employee work in Baltimore city government is still less than the mean. 

_Cluster 3 node_, which is Mechanical Maintenance Technical Superviser II, has positive z scores for years worked, gross pay, and annual salaries in FY2020. It has the highest years worked among all the cluster nodes, but has lower gross pay and annual salaries than that of cluster 2 and 4 nodes. Jobs in this cluster have high retention rate even when the pay is not as high. 

Lastly, _cluster 4 node_, which is finance project manager, has lowest z-scores for years worked and highest z scores for gross pay and annual salaries in FY2020 among all the clusters. This means that jobs in this cluster have the highest pay, but the retention rate is still low. 

### What are the characteristics of each cluster by years worked and gross pay in FY2020?

<img width="881" alt="Screen Shot 2021-03-16 at 6 19 02 PM" src="https://user-images.githubusercontent.com/70459912/111387462-20430400-8684-11eb-984b-1b7f48d0eec7.png">
<img width="1187" alt="Screen Shot 2021-03-16 at 6 24 18 PM" src="https://user-images.githubusercontent.com/70459912/111387885-d4448f00-8684-11eb-9ae5-ff18ea3513a6.png">

Similar results to the analysis of nodes can be drawn here. As shown in the graph, jobs in cluster 1 are low in both gross pay and years worked, with the average years worked of 11.052 year and average gross pay of 41690. There are total of 503 jobs (48.8%) in this cluster. Jobs in cluster 2 have an average of 81438 USD of gross pay in FY2020 and 13.820 years worked, which is the second highest in gross pay and second lowest in years worked. There are 267 jobs in this cluster, representing 25.9% of the jobs in Baltimore city government. On the other hand, in cluster 3, the average gross pay of jobs is 76874 and the average years worked is 33.193, which is second lowest in gross pay and highest in years worked. There are 179 jobs in this category, representing 17.4% of the jobs in Baltimore city government. Lastly, in cluster 4, the average gross pay of jobs is 137587 USD and average years worked is 14.672 years. There are total of 82 jobs (7.95%) in cluster 4.

## Business Answer
Based on the analysis, it is interesting to see that higher salary won't necessarily retain more employees. In cluster 4, although these jobs are well paid, the years worked is still below average, while in cluster 3, the employees tend to stay longer at the job even though the pay is quite low. To understand the reasons behind such unintuitive phenomena, the Baltimore police department can investigate other variables such as hours worked per day, benefits, work culture, etc. of jobs that fall in cluster 3 to see if there are any particular reasons for high retention rates. Baltimore city government can also look into the reasons why the jobs in cluster 4 have high turnover rates even though the pay is competitive. With these further research, the Baltimore city government can better correlate employee retention rate with other variables and design policies to encourage employees to stay at their jobs and boost productivity.    


