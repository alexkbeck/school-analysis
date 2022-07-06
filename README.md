> # California School Affordability Analysis

![California](https://www.greatvaluecolleges.net/wp-content/uploads/2021/04/Top-15-Cheapest-Colleges-in-California.jpg)

California is the largest state in the U.S. and has a diverse population, climate, and culture. Housing is notoriously expensive in California. School funding is driven in part by the property taxes of the area that the shcool serves. This leads to better funded schools in neighborhoods with higher housing prices. The purpose of this ananlysis is to compare school performance against housing prices with the goal of finding locations where school performance is high and housing prices are relatively low. In this analysis income is factored into the housing price calculation to get a housing affordability ratio. Areas with high housing prices also tend have higher relative incomes, so I want to control for that. I am personally interested in the outcomes of this analysis and I have a college degree, so I will be considering the median income of college graduates only.

School performance is defined across these dimensions:  
* Greatschools.org rating  

Housing affordability is defined across these dimensions:  
* Median house price
* Median income for college graduates

The metric that we are trying to evaluate could be expressed as the following (higher score is better):  
`school_affordability_index = greatschools_rating / (median_house_price / median_income)`

This analysis will calculate the `school_affordability_index` for each ZIP code in California. Choropleth maps will be at the end of the analysis to help readers visualize the effect of geography on the metric.

*Note: this notebook does not contain code for the intermediary steps of analysis, ie. inspecting the data, troublshooting joins, etc. This notebook is intended to showcase my work and I want to make it enjoyable to read end-to-end. My intention is not to come off hand-wavey, so just know there was a lot of work done that were the building blocks of the code and analysis you find below.*
