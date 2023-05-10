# ppol670_final
Repository for PPOL 670 Final Project

*This project was completed in fulfillment of the 'Intro to Data Science' final group project for the Spring 2023 semester by Ben Burnley, Sean Conner, Gustavo Murillo Velazquez, & Katie Ward.* 

Our initial research question sought to investigate how redistricting affected voter turnout at the precinct level in a state where significant redistricting occurred. We chose Florida given its national profile of a state with one-party control of the three branches of government and its notable efforts to redistrict following the 2020 Census. 

Our datasets came from the [Redistricting Hub](https://redistrictingdatahub.org/). We were able to pull the data using an API that required registration, approval, and the utilization of a Jupiter notebook in Python. Unfortunately, we discovered that precinct-level voter turnout has not been released as shapefiles for the 2022 election yet. This made comparison for voter turnout specifically between the new and prior districts not feasible. However, we were still able to do considerable analysis pulling from available data. 

### Data Visualizations
The data was cleaned and wrangled to merge precinct-level election results with whether or not the precinct was redrawn in 2022. We used geospatial analysis to overlay the 2018 and 2022 districts, as well as visualize which specific precincts were redrawn into different districts. We also mapped electoral results from 2018 for the precincts that were redrawn. 

### Modeling
We then used our data to develop a model to predict whether election results from 2018 could predict the likelihood of a precinct being redrawn. We employed a logistic regression with cross-validation and a random forest model with cross-validation and hyperparameter tuning. We then measured the results of these models and finalized a best-fit model based on an ROC curve. We created a variable importance matrix, which revealed Districts 5 and 13 have the most predictive power in our model to predict if a precinct is redrawn. Upon running further geospatial analysis, we can see these districts are predominantly black and gets splits/dispersed into other districts in the 2022 map. 

### Reflection and Next Steps
This project revealed the challenging nature of understanding characteristics at the precinct level and merging datasets of different geographic boundaries. Further demographic analysis could not be easily completed because census data is done at either district and tract levels, as well as precinct-level data was not yet available for the time period we were most interested in. Further analysis could try to be accomplished through attempting to merge and connect various shapefiles, waiting on the 2022 precinct-level data to come out, and examining other states for similar patterns. 

Link to GitHub Page: https://benjaminrburnley.github.io/ppol670_final/
