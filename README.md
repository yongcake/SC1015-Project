# SC1015-Project
This project aims to analyze Kickstarter data to predict the success of a kickstarter project. 

## Motivation: 
Kickstarter serves as a platform for innovators, creators, and entrepreneurs to bring their project ideas to life. However, there are always uncertainty and risks that comes with backing a project, as some projects has higher potential for success while some are more likely to fail. Using ML to analyze historical data on kickstarter projects, we can develop a predictive model that can forecast the success of a kickstarter project, so that investors or supporters can have better decision making when it comes to choosing which project to support.

The data set for this project can be found at https://www.kaggle.com/datasets/kemical/kickstarter-projects/data?select=ks-projects-201801.csv 

## Dataset columns
ID - Internal Kickstarter ID <br>
name - name of the project<br>
category - sub category that the project belongs to<br>
main_category - main category of campaign (sub category falls into main category)<br>
currency - currency used to support<br>
deadline - deadline to crowdfunding<br>
goal - the fundrasing goal is the amount of money that a creator needs to complete their project<br>
launched - data launched<br>
usd_pledged - pledged amount in USD (conversion made by kickstarter)<br>
usd_pledged_real - pleadged amount made in USD (conversion made by fixer.io api)<br>
state - current condition the project is in<br>
backers - number of backers <br>
country - country pledged from <br>
usd_pledged - amount of money pledged in USD<br>
goal - target amount that the creators want, success is determined if pledged > goal<br>
usd_goal_real - Goal amount in USD (conversion made by fixer.io api)<br>

