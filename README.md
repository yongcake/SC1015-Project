# SC1015-Project
This project aims to analyze Kickstarter data to predict the success of a kickstarter project. 

## Motivation: 
Kickstarter serves as a platform for innovators, creators, and entrepreneurs to bring their project ideas to life. However, there are always uncertainty and risks that comes with backing a project, as some projects has higher potential for success while some are more likely to fail. Using ML to analyze historical data on kickstarter projects, we can develop a predictive model that can forecast the success of a kickstarter project, so that investors or supporters can have better decision making when it comes to choosing which project to support.

The data set for this project can be found at https://www.kaggle.com/datasets/kemical/kickstarter-projects/data?select=ks-projects-201801.csv 

## Dataset columns
ID - Internal Kickstarter ID
name - name of the project
category - sub category that the project belongs to
main_category - main category of campaign (sub category falls into main category)
currency - currency used to support
deadline - deadline to crowdfunding
goal - the fundrasing goal is the amount of money that a creator needs to complete their project
launched - data launched
usd_pledged - pledged amount in USD (conversion made by kickstarter)
usd_pledged_real - pleadged amount made in USD (conversion made by fixer.io api)
state - current condition the project is in
backers - number of backers 
country - country pledged from 
usd_pledged - amount of money pledged in USD
goal - target amount that the creators want, success is determined if pledged > goal
usd_goal_real - Goal amount in USD (conversion made by fixer.io api)

