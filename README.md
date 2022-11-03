# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1: Standardized Test Analysis

### Liam Ting Wei, SG-DSI33

### Problem Statement

Standardized testing remains a topic of controversy today. One of the arguments against requiring standardized test scores in college admissions is that students from wealthier backgrounds can afford better test prep and thus achieve higher scores on them. These tests may thus be seen as discerning family wealth rather than aptitude. Do states with higher median family income thus do better at the ACT and/or SAT?

### Summary
This project aims to explore trends between family income levels and standardized test scores at an inter-state level to enable colleges to make better informed decisions on whether to use these test scores as part of their admissions criteria.

State ACT composite score increases as state median family income increases. This supports the argument that wealth has a positive influence on ACT test scores, and there might be some issues with fairness.

No significant trend between SAT total score and median family income was found. States with higher median income can have SAT scores than those with lower median incomes, suggesting that SAT scores might actually be a more equitable measure of aptitude that is less influenced by wealth.

That being said, states with higher median family income appear to lean more towards the SAT. The reverse is true for the ACT since ACT and SAT participation rates are negatively correlated. 

### Conclusions and Recommendations
The data suggests that wealthier states have higher mean ACT composite scores, while no such relationshp is seen with SAT total scores. This could serve as a starting point to re-evaluate the validity of the ACT in being an objective measure of academic aptitude or find interventions to uplift lower median income states.

Of note is also the fact that ACT participation is higher with lower state median family income, which means overhauling the way schools approach the ACT could have greater impact. While it is way more difficult to tackle income disparity to level the playing field in the short run, better basic test preparation for the ACT can be implemented in schools within a shorter time frame as a means to bridge the resource gap. Learning points could be picked up from the Chinese GaoKao, a nationwide standardized test used for college admissions in China. There, the final year of high school is often devoted to preparations.

While standardized testing may not exactly be the fairest of measures, neither are other college admission criteria. Coming from a wealthier family is likely to provide more opportunities for extracurricular activities, relevant work opportunities, and volunteering experiences as well.

Back in 2014, the College Board reviewed and overhauled the SAT tests. Data back then showed a positive correlation between students' household incomes and SAT test scores. Perhaps the overhaul had its intended effect, making the SATs a much more equitable measure of aptitude based on 2019 data. Colleges should thus consider using the SAT as a part of its admissions criteria.

### Data

2019 ACT and SAT data provided as part of project materials
* [`act_2019.csv`](./data/act_2019.csv): 2019 ACT participation rates and composite scores by state
* [`sat_2019.csv`](./data/sat_2019.csv): SAT participation rates and scores by state

Income data for US states were sourced from the American Community Survey
* [`us_income_2019.csv`](./data/us_income_2019.csv): 2019 median household/family/per capita income by state extracted from US census 2020 data; source https://data.census.gov/

Data Dictionary
|Feature|Type|Dataset|Description|
|---|---|---|---|
|**state**|*string*|merged|A US state|
|**median_family_income**|*integer*|merged|Median income of families| 
|**per_capita_income**|*integer*|merged|Median per capita income| 
|**act_participation**|*float*|merged|Percentage of high school students who took the ACT| 
|**act_composite_score**|*float*|merged|Composite score for ACT; Average of all the tests|
|**sat_participation**|*float*|merged|Percentage of high school students who took the SAT|
|**sat_total_score**|*float*|merged|Total SAT score; sum of math and ebrw tests|
|**sat_ebrw**|*float*|merged|Score for SAT ebrw test|
|**sat_math**|*float*|merged|Score for SAT math test|
