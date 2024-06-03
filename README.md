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

I then checked the OLS regression results for each and wrote out an interpretation (found in "Regression RDD Project - Neil Aucoin") to have a good idea each cutoff's impact on the data. 
 
 Having some promising results, I compiled all of the cutoffs into one complete timeline along with a number of potentially relevant events that could have also affected covid statistics to allow further understanding of the context surrounding our cutoffs.  
   
![Full Timeline](https://github.com/NeilAucoin/Regression-Discontinuity-Design-Project---COVID-Cases-in-Quebec/blob/main/assets/Full_Timeline.PNG?raw=true)

# Results
## Initial Lockdown
Regression results and chart analysis would indicate that the initial lockdown correlated with a significant increase in COVID cases, however we can infer that this is a biased result as this took place during the first days of the pandemic where COVID cases were bound to increase significantly regardless of measures taken. As such, results for this measure are inconclusive.

![Cutoff 1](https://github.com/NeilAucoin/Regression-Discontinuity-Design-Project---COVID-Cases-in-Quebec/blob/main/assets/Cutoff_1.png?raw=true)

## Reopening of Schools
Charts and OLS regression results indicate that the reopening of schools on 31/8/2020 correlated with a significant increase in covid cases. We can see in the chart below that cases had largely evened out to a relatively low rate and had just begun to increase again when schools were reopened, after which the rate of COVID cases skyrocketed. All of this indicates that schools reopening were in part, if not largely responsible for a significant number of COVID cases.

![Cutoff 2](https://github.com/NeilAucoin/Regression-Discontinuity-Design-Project---COVID-Cases-in-Quebec/blob/main/assets/Cutoff_2.png?raw=true)

## Holiday Lockdown
Looking at the short-term effects of the holiday lockdown, it seems to have had little immediate effect; however, we can infer that this rise in COVID cases was inevtiable as many gatherings took place during the holiday season regardless of regulations against them. Looking further down the timeline, COVID cases dropped significantly, which may be a direct result of the new lockdown regulations (as well as the end of the holiday season). While OLS regression results are inconclusive for this cutoff, we can infer that the lockdown helped curb COVID cases to an extent, as many individuals likely refrained from having large holiday gatherings due to these restrictions and COVID cases continued to decrease significantly after the holidays (while the new lockdown was still in effect).

![Cutoff 3](https://github.com/NeilAucoin/Regression-Discontinuity-Design-Project---COVID-Cases-in-Quebec/blob/main/assets/Cutoff_3.png?raw=true)

# ---
Full regression reuslts and interpretations can be found in "Regression RDD Project - Neil Aucoin.ipynb" and "Regression Discontinuity Design Project.pptx"
