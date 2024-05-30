# Project Explanation
Use RDD to estimate the effectiveness of the following COVID-related events in Quebec:

1. The 20/3/2020 lockdown
2. The reopening of schools on 31/8/2020
3. The 25/12/2020 lockdown

# Solution
Link to Data and Data Dictionary:
- https://open.canada.ca/data/en/dataset/261c32ab-4cfd-4f81-9dea-7b64065690dc

Link to COVID event timelines:
- https://montrealgazette.com/news/local-news/covid-19-timeline-a-year-like-no-other-in-quebec 
- https://www.who.int/emergencies/diseases/novel-coronavirus-2019/interactive-timeline#!

I started off by extracting the relevant data from the Government of Canada Public Health Infobase COVID statistics database, then defined my cutoff dates (Quebec COVID measure dates) in order to create my treatment variables (before and after each cutoff). Afterwards, I created some basic RDD plots for each cutoff.  
  
![Cutoff 1](https://github.com/NeilAucoin/Regression-Discontinuity-Design-Project---COVID-Cases-in-Quebec/blob/main/assets/Cutoff_1.png?raw=true)

![Cutoff 2](https://github.com/NeilAucoin/Regression-Discontinuity-Design-Project---COVID-Cases-in-Quebec/blob/main/assets/Cutoff_2.png?raw=true)

![Cutoff 3](https://github.com/NeilAucoin/Regression-Discontinuity-Design-Project---COVID-Cases-in-Quebec/blob/main/assets/Cutoff_3.png?raw=true)

I then checked the OLS regression results for each and wrote out an interpretation (found in "Regression RDD Project - Neil Aucoin") to have a good idea each cutoff's impact on the data. 
 
 Having some promising results, I compiled all of the cutoffs into one complete timeline along with a number of potentially relevant events that could have also affected covid statistics to allow further understanding of the context surrounding our cutoffs.  
   
![Full Timeline](https://github.com/NeilAucoin/Regression-Discontinuity-Design-Project---COVID-Cases-in-Quebec/blob/main/assets/Full_Timeline.PNG?raw=true)

Full explanation of results and interpretations can be found in "Regression RDD Project - Neil Aucoin.ipynb" and "Regression Discontinuity Design Project.pptx"
