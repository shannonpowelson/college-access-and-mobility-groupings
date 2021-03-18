# Grouping Colleges based on Mobility Rates and Related Metrics
## Background
For this analysis, I studied how colleges are grouped based on mobility and other related metrics.  The mobility rate is defined by [Opportunity Insights](https://opportunityinsights.org/) as the "percent of students who have parents in the Bottom 20% of the income distribution and reach the Top 20% of the income distribution".  Colleges have the potential to facilitate this mobility.  Some colleges do this better than others.  In one [research study](https://www.brookings.edu/research/opportunity-engines-middle-class-mobility-in-higher-education/), colleges with higher instructional expenditures per student were found to be associated with higher mobility rates.  But are these schools accessible to students who have parents in the bottom 20% of the income distribution?  Does high tuition and rejection rates inhibit these students from getting into a college with high mobility rates?  These questions are explored in a cluster analysis that groups colleges based on mobility rate, fraction of parents in the top 1% of the income distribution, rejection rate, and instructional expenditures per student.  On the contrary, another [article](https://www.forbes.com/sites/prestoncooper2/2020/07/15/which-colleges-are-fulfilling-the-promise-of-intergenerational-mobility/?sh=22e2596163bc) claimed that high mobility rates are hindered by higher instructional expenditures per student and instead are associated with certain majors like engineering and business.  This claim is explored through another cluster analysis that groups colleges based on major and mobility rates.  

## Business Question
_How are colleges grouped based on mobility rates and related metrics?_

## Data Sources 
1. College Level Characteristics
https://github.com/shannonpowelson/college-mobility-groupings/blob/main/College%20Level%20Characteristics.xlsx
This data is from Opportunity Insights and it contains the institutional expenditures per student in 2012, the share of students in each major grouping in 2000, and the rejection rates in 2013 for each college.  

2. Preferred Estimates of Access and Mobility Rates by College
https://github.com/shannonpowelson/college-mobility-groupings/blob/main/Preferred%20Estimates%20of%20Access%20and%20Mobility%20Rates%20by%20College.xlsx
This data is from Opportunity Insights and it contains the mobility rates and the fraction of parents in the top 1% of the income distribution for each college.  

3. Cluster_Analysis_One_Data
https://github.com/shannonpowelson/college-mobility-groupings/blob/main/Cluster_Analysis_One_Data.xlsx
This file contains the data, cluster analysis, and visualization for the cluster analysis that groups colleges based on mobility rate, fraction of parents in the top 1% of the income distribution, rejection rate in 2013, and institutional expenditures per student in 2012.  

4. Cluster_Analysis_Two_Data
https://github.com/shannonpowelson/college-mobility-groupings/blob/main/Cluster_Analysis_Two_Data.xlsx
This file contains the data, cluster analysis, and visualization for the cluster analysis that groups colleges based on mobility rate, arts and humanities major share, business major share, health and medicine major share, multi/interdisciplinary studies major share, public and social services major share, STEM major share, social sciences major share, and trades and personal services major share in 2000.  

## Data Analysis
To start this analysis, I performed a cluster analysis that grouped colleges based on mobility rate, fraction of parents in the top 1% of the income distribution, rejection rate, and instructional expenditures per student.  The images below show the results of the 4 anchor cluster analysis that was performed.  In the bar graph, the y=0 line represents the average for each variable.   

![alt text](https://github.com/shannonpowelson/college-mobility-groupings/blob/main/Cluster_Analysis_One.png)
![alt text](https://github.com/shannonpowelson/college-mobility-groupings/blob/main/visualization_two.png)

The first cluster has an above average mobility rate and rejection rate.  It also has a below average fraction of parents in the top 1% of the income distribution and below average instructional expenditures per student.  The second cluster has an above average rejection rate and a below average mobility rate, fraction of parents in the top 1% of the income distribution, and instructional expenditures per student.  The third cluster is below the average for all of the variables.  The fourth cluster is below average for the mobility rate, but above average for the other variables.  

As shown in these results, the only cluster that is above average for the instructional expenditures per student is below average for the mobility rate.  Also, the only cluster that is above average for mobility rate is the most below average for instructional expenditures per student.  Since this contradicted the initial research study that I read about, I looked into this topic some more and found the previously mentioned article that discussed how the type of major is associated with mobility rates.  

To explore this claim, I performed another cluster analysis that grouped colleges based on the share of students in each grouping of majors at each college and the mobility rate.  The following groups of majors were used: Arts and humanities, business, health and medicine, multi/interdisciplinary, public and social services, STEM, social sciences, and trades and personal services.  The images below show the results of the 4 anchor cluster analysis that was performed.  In the bar graph, the y=0 line represents the average for each variable. 

![alt text](https://github.com/shannonpowelson/college-mobility-groupings/blob/main/Cluster_Analysis_Two.png)
![alt text](https://github.com/shannonpowelson/college-mobility-groupings/blob/main/visualization_one.png)

An interesting finding from this analysis is that colleges that have an above average share of arts and humanities majors are grouped with colleges that have above average mobility rates.  

## Summary 

The first cluster analysis showed that colleges with below average instructional expenditures per student are grouped with above average mobility rates, while colleges with above average instructional expenditures per student are grouped with below average mobility rates.  This shows that there is a possibility that there is an association between low mobility rates and high instructional expenditures.  These groupings cannot be used to prove an association, so linear regression should be used to further this analysis.  In addition, the second cluster analysis showed that only one cluster had an above average mobility rate and that in this cluster, the only major that was above average was the arts and humanities major.  This is interesting, because it is normally assumed that students pursuing STEM or business majors get higher paying jobs than the arts and humanities majors and therefore would have higher mobility rates.  Colleges should research this to see the programs in this major and these schools in this cluster.  There could be various variables that are improving student outcomes and thus mobility rates.  The school could have many networking events, more startup funding opportunities, and a location with more jobs.  Another question for further research is do these students from this major pursue the industry of their major?  Overall, these analyses demonstrate that in order to improve mobility rates, colleges should be thinking about the quality and long term impact of the majors and programs they offer to students instead of just the quantity of money that they spend on students.  



