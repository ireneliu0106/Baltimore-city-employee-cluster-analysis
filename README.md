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
Here are the [Excel file for data analysis] and the [step-by-step descriptions of Excel data analysis]

The dataset does not explicitly contain the data for years worked in Baltimore city government of each employee. Therefore, it was calculated by subtracting 3/18/2021 by the hire date of each employee. 4 anchor nodes were used in the cluster analysis to categorize the jobs into 4 main groups with different characteristics of years worked, gross pay, and annual salary. 

### __What are the characteristics of each cluster?__
<img width="888" alt="Screen Shot 2021-03-16 at 12 53 29 PM" src="https://user-images.githubusercontent.com/70459912/111348466-9df01b00-8656-11eb-80de-7d61b8f12db3.png">
<img width="1180" alt="Screen Shot 2021-03-16 at 12 54 07 PM" src="https://user-images.githubusercontent.com/70459912/111348561-b4967200-8656-11eb-9ca0-5e3f59039fe2.png">

As shown in the graph, _cluster 1_ with anchor node of the job Control System Operator is characterized by the low years worked in Baltimore city government, lowest gross pay, and lowest annual salaries. The z scores of all three variables in this cluster are negative, meaning that the jobs fall in cluster 1 have years worked, gross pay, and annual salaries in FY2020 lower than the mean. There are total of 503 jobs (48.8%) in this cluster.

On the other hand, _cluster 2_ with anchor node of the job F&P Benefits Analyst Superviser has negative z scores for years worked and positive z scores for gross pay and annual salaries in FY2020. There are 267 jobs in this cluster, representing 25.9% of the jobs in Baltimore city government.

In _cluster 3_, the anchor node is Mechanical Maintenance Technical Superviser II, which has positive z scores for years worked, gross pay, and annual salaries in FY2020. It has the highest years worked among all the cluster, but has lower gross pay and annual salaries than that of cluster 2 and 4. There are 179 jobs in this category, representing 17.4% of the jobs in Baltimore city government.

Lastly, in _cluster 4_, the z-scores for years worked is the lowest while the z scores for gross pay and annual salaries in FY2020 is the highest among all the clusters. This means that jobs in this category have the highest pay, but the retention rate is still low. There are total of 82 jobs (7.95%) in this cluster.


