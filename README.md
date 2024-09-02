# SalifortMotorsAnalysis
This project was the final assignment I completed in order to obtain my Google Advanced Data Analytics certification through Coursera. In this scenario, I was working for a fictional company, Salifort Motors. They had been having a problem with a high turnover rate and they wanted me to investigate the possible causes why. This assignment involved drafting a project proposal, conducting the data analysis, and drafting a one-page summary of my results. 

## Project Proposal
This proposal involved breaking the most significant steps of my data analysis into milestones so that I could present them to other people before I started working. Each milestone was also assigned to part of the PACE framework. PACE is an acronym where each letter represents a different stage in the project: plan, analyze, construct, and execute. Understanding the scope of the problem, research, and acquiring data are examples of the planning stage. Data exploration, data cleaning, and evaluating model results would be examples of the analysis stage. Constructing the model and adjusting the model as you evaluate its results are examples of the constructing stage. Finally, interpreting model results and sharing results are examples of the execution stage.   

## Data Analysis
The Data Analysis started by gathering basic information about the dataset using the .info() and the .describe() functions. These functions told me some important information like the datatypes of the columns I was working with and statistical information like the mean, min, and max of each column. Next, I conducted some data cleaning. I renamed my columns to standardize lower case, snake casing, and made the names of columns more concise. I also checked if I need to remove any missing columns or duplicate columns. The next stage of my analysis was creating a series of data visualizations to better examine the data I was interested in. These visualizations often revealed that the employees who left had worked a very large number of hours, taken on a large number of projects, or been at the company for many years without a promotion. For example, a stacked box plot showed that every employee who worked on 7 projects at a time left the company and another plot showed that every employee who worked over 300 hours a month without a promotion in the last 5 years left the company. A correlation heatmap also confirmed these results. There was a significant negative relationship between satisfaction level and 'number_project', 'average_monthly_hours', and 'tenure'. The next stage in my data analysis was constructing a model. My goal was to predict whether or not an employee will leave the company or not. Therefore, I was attempting to predict a binary categorical outcome variable. I decided to create a logistic regression model. Since logistic regression is sensitive to outliers, I had to remove outliers from the tenure column. Another important part of constructing a logistic regression model is splitting the data into training and testing data so the model can cross-validate the resulting data. The result was a confusion matrix where the top half was employees the model predicted would stay and the bottom half was employees the model predicted would leave. The model was also very balanced with a 45-55% class split. 

## Insights and Final Summary
The Data shows that many employees in the company feel overworked. The data visualizations often showed a negative relationship between employee satisfaction and average monthly hours, number of projects, and tenure. The data also showed that employees that took on many projects or worked a large number of hours were still unlikely to receive a promotion, further adding to feelings of burnout. I kept this in mind when coming up with recommendations for the future in the final summary. In the final summary I started by discussing the problem of the company's high turnover rate and the response to create a logistic regression model. I shared how this model can help predict the likelihood that an employee will leave. I also provided two visualizations. The first was a heatmap that showed the relationships between certain variables in the company. This showed the many negative relationships that existed between things like employee satisfaction. The second was the confusion matrix showing the accuracy of the logistic regression model. Finally, I provided recommendations for the company moving forward. Some of these were placing a cap on the number of projects an employee can work on, considering promoting employees who had worked with the company for several years, and providing more rewards to employees for working extra hours. 
