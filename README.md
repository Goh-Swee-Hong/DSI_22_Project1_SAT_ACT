# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1:  SAT & ACT Analysis

## Background

The ACT was created by an education professor at the University of Iowa named Everett Franklin Lindquist in 1959 as a competition to SAT. It was administered to 75460 students in the first year it was created. It gained popularity and grew the number to over a million in 1972. By 2015, ACT has surpassed SAT as the most popular college admissions test. In 2016, a new format of SAT with less confusing question phrasing and trigonometry in the math section was released.

## Problem Statement

To make recommendations to the College Board about how the Board might work to increase the participation rate in a state of my choice.


## Executive summary

> The new format for the SAT was released in March 2016. As an employee of the College Board - the organization that administers the SAT - you are a part of a team that tracks statewide participation and recommends where money is best spent to improve SAT participation rates. Your presentation and report should be geared toward **non-technical** executives with the College Board and you will use the provided data and outside research to make recommendations about how the College Board might work to increase the participation rate in a **state of your choice**.

Contents:
2017 Data Import & Cleaning
2018 Data Import and Cleaning
Exploratory Data Analysis
Participation rates
Making comparisons with participation rates
Making comparisons using difference in participation rates between 2017 and 2018
States with more than 50% participation rate in both years
Total/composite score
Summary from EDA
Data Visualization
Descriptive and Inferential Statistics
Outside Research
Conclusions and Recommendations

### Datasets

#### Provided Data

2017 and 2018 SAT and ACT data were provided as a part of project materials.

#### Additional Data

https://blog.prepscholar.com/the-history-of-the-act-test#:~:text=Overview,sections%20were%20created%20in%201989.
https://www.census.gov/data/datasets/time-series/demo/popest/2010s-counties-total.html#par_textimage_70769902
https://educationdata.org/public-education-spending-statistics
---

#### Updated data dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|state|object|final3|State name|
|participation_sat2017|int|final3|Participation rate of the State in 2017 in %| 
|read_write2017|int|final3|Average Evidence-based reading and writing score of the State in 2017| 
|math_sat2017|int|final3|Average Math score of the State in 2017| 
|total_sat2017|int|final3|Average total score of the State in 2017| 
|---|---|---|---|  
|participation_act2017|int|final3|Participation rate of the State in 2017 in %|
|english_2017|float|final3|Average English score of the State in 2017| 
|math_act2017|float|final3|Average Math score of the State in 2017|
|reading_2017|float|final3|Average Reading score of the State in 2017|
|science_2017|float|final3|Average Science score of the State in 2017|
|composite_2017|float|final3|Average Composite score of the State in 2017|
|---|---|---|---|
|participation_sat2018|int|final3|Participation rate of the State in 2018 in %| 
|read_write2018|int|final3|Average Evidence-based reading and writing score of the State in 2018| 
|math_sat2018|int|final3|Average Math score of the State in 2018| 
|total_sat2018|int|final3|Average total score of the State in 2018| 
|---|---|---|---|  
|participation_act2018|int|final3|Participation rate of the State in 2018 in %|
|english_2018|float|final3|Average English score of the State in 2018| 
|math_act2018|float|final3|Average Math score of the State in 2018|
|reading_2018|float|final3|Average Reading score of the State in 2018|
|science_2018|float|final3|Average Science score of the State in 2018|
|composite_2018|float|final3|Average Composite score of the State in 2018|
|diff_participation_sat|int|final3|Difference in participation rates in SAT between 2017 and 2018|
|diff_participation_act|int|final3|Difference in participation rates in ACT between 2017 and 2018|
|population|int|final3|Population of the State in 2019|
|spend|int|final3|Spending per pupil in each State in 2019|

## Conclusions and Recommendations

The objective is to make recommendations to the College Board about how the Board might work to increase the participation rate in a state of my choice.

Approaching the issue from three angles:
1. States with lower participation rate in SAT so growth potential is higher as there will be more room for conversion.
2. States with relatively higher population. Higher population equates to a wider target audience.
3. States with higher spending budget allocated per pupil implies the level of importance a State places on academic.

There are a total of 18 States with participation rate of 10% and below in SAT in 2018 and they are Tennessee, Missouri, Wisconsin, Minnesota, Alabama, Louisiana, Kentucky, Oklahoma, Utah, Iowa, Arkansas, Mississippi, Kansas, Nebraska, Montana, South Dakota, North Dakota, Wyoming in the order of descending population size. 

From the list, Minnesota is the 4th most populated State with the 3rd highest spending per pupil. Having only 4% participation rate in SAT in 2018 show that there is a huge room for improvement. The 1% increment in the participation rate from 2017 which, while small, indicated that Minnesota is positively receptive of SAT.

Using a push and pull approach, the Board will push by working with the Education department of Minnesota to implement SAT statewide. The newly revamped SAT will provide Minnesota, as an admission exam, with a more reliable performance assessment for colleges and public universities to use to guide student placement. Following up, the Board will pull by placing focus on social media marketing to target high school students and their parents to further strengthen acceptance.

With the three angles of consideration coupled with the push and pull approach, Minnesota, a State with low participation rate in SAT, relatively high population and high spending per pupil is the State for the Board to expend resources into increasing the participation rate.

