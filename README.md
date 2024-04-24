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

## Data Preparation and Cleaning
In this part of the project we prepared and cleaned the dataset to help analyze our data better and also make the data more suitable to be used for purposes of machine learning in the later sections.

We performed the following:
1. Checking and dropping any NULL values in the dataset. (in the 15 variables)
2. Dropped all the unwanted columns. ( 7 variables dropped )
3. Split the columns with datetime ("deadline" and "launched") into seperate columns with the month,year and duration of campaign.
4. Remove all state types other than "successful" and "failed" due to ambiguity in them.
5. Encoding the categorical variables.

## Exploratory Data Analysis

Then, we continued on to using Exploratory Data Analysis to find patterns in our data and answer some questions like What do our success variables look like? What is the general trend in the relationship between variables?  Can we make any inferences for our question at this stage?

To achieve this we performed the following:

Analysis of numerical variables:
1. Compare goal amount with the states and move on to determine success rate by goal amount range
2. Explore duration of campaign in days and the success rate vs the state
3. Explore number of backers and the success rate vs the state
4. Compare the pledged amount in usd with the success rate



Analysis of categorical variables:
1. Plot the success rate and the main categories to find a relation , and then seperate the categories to succesfull and 
   failed campaigns and analyze the role of main categories with respect to this.
2. Explore the relation of countries with the success rate of the startup campaign.

## Models 
1. DecisionTreeClassifier
2. RandomForestClassifier
3. XGBoost Classifier

## Conclusion 
- From EDA, we found the variables with higher correlation through visualization, to predict the success or failure of the kickstarter projects
- We were able to reach a accuracy of 93% with XGBoost Classifier

## Learning Outcomes


## Contributions 
- Yee Yong Khang [yongcake](https://github.com/yongcake) - README, EDA, XGBClassifier Tuning
- Shah Mihir Sunil [mihirshah2005](https://github.com/mihirshah2005) - 
- Tan Yong Huat [TenLetterx](https://github.com/TenLetterx) -

## References
- https://www.kaggle.com/datasets/kemical/kickstarter-projects/data?select=ks-projects-201801.csv


