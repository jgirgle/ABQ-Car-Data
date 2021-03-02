Albuquerque Vehicle Emissions Analysis

Research Questions:

   1)	Is there a predictable linear trend in emissions test failure rate vs. vehicle age?
   2)	Is there a statistically significant difference in the performance of certain models, compared to the population average, on a vehicle-age basis?

Data Set Overview:

Albuquerque Vehicle Emissions Database
  ●	Environmental Health Department / Vehicle Pollution Management 
  ●	A record of every emissions test in the city
  ●	Abundance of data (~257,000 records per year):
    ○	2013: 257,673;  2014: 258,985;  2015: 257,790;  2016: 259,865;  2017: 251,397
  ●	We used a reduced dataset:
    ○	based on 2014-2017 data
    ○	50 or more records (make/model/year)
    ○	represents 822,763 individual reports
    ○	only consider pass/fail status

Methodology

A) Piecewise Linear Regression (weighted1)
  ●	independent variable: vehicle age (years)
  ●	dependent variable: failure rate
  ●	weighted based on number of vehicles in each category
B) Large-sample hypothesis test of proportions
  ●	“Does a vehicle of specific make/model/age perform better or worse than typical vehicle of the same age?”
  ●	Assume population is total available dataset
  ●	H0: p[vehicle,age] = p[age]
  ●	Ha: p[vehicle,age] > p[age] or p[vehicle,age] < p[age]


Database: Excel
Tools: Pivot Tables / LOOKUP Functions / Linear Regression / Charting
