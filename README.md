Football analytics (FIFA 2020)¶
Content
Different Analysis for FIFA 2020 players database provided by Kaggle (https://www.kaggle.com/stefanoleone992/fifa-20-complete-player-dataset?select=players_20.csv)
##### Data wrangling process:
Remove some unnecessary data as the current version is 14.5+ MB
Check duplicated values
ooking for the first 10 rows we can find that the we do not need core change/correction for the data types nor the columns names


What is the structure of your dataset?
After the filtertaion of dublicated and unnessacry data we have 18278 sample/row for 100 features/column.

What features in the dataset do you think will help support your investigation into your feature(s) of interest?
I will work on comperhensive study for the relationships between different features that affect performance and reputation of the football player.

It is predictable that the player's Position,Age, Weight, Height, and Potential would affect his International Reputation,Value, and Wage.

What is/are the main feature(s) of interest in your dataset?
My study includes these : Position,Age, Weight, Height,Potential, International Reputation,Value, and Wage.


## Summary of Findings

Univariate Exploration
A series of plots. Initial Insights: 1.The max international reputation is 5 and the minimum one is 1. 75% of the players has 1 as international reputation. 2.The max age is 42 years old and the min one is 16 years old.75% of the players are around 29 years old 1. 3.The max height is 205 cm and the min one is 156 cm.75% of the players are around 186 cm. 4.The max weight is 110 kg and the min one is 50 kg.75% of the players are around 80 kg.

Discuss the distribution(s) of your variable(s) of interest. Were there any unusual points? Did you need to perform any transformations?¶
Basic Factors
Weight, hieght and potential distributions are normal.
Age 's distribution is slightly positively skewed. This support the initial finding of mean is greater than median and median greater than the mode.
Categorical Factors
Most of the players have the same international reputation(So no need for extra study on this factor),
There are no big differences between Values and wages of the top five players.The distribution of values and wages are almost the same.(So a study on the value is Enough) -Most of the players are in the sub position.
Of the features you investigated, were there any unusual distributions? Did you perform any operations on the data to tidy, adjust, or change the form of the data? If so, why did you do this?
I tried to remove all the features/ columns that have missing data to get correct analysis.


Bivariate Exploration
Let's have a look at correlations


Talk about some of the relationships you observed in this part of the investigation. How did the feature(s) of interest vary with other features in the dataset?
-There is a clear positive(exponential) relationship between potential and value. -There are optimum margins of Age, height and weight to get high-valued player. -There is a slight positive correlation between weight and height. -There is a negative correlation between age and potential. Each Finding supports the others to reach to one main title for this part of analysis:There are optimum margins of Age, height and weight to get high valued player.

Did you observe any interesting relationships between the other features (not the main feature(s) of interest)?
Surpisingly players who play Right-forward positions are valued more than other positions. Then the Right-wing back and Left-wing back are valued lowest.


Multivariate Exploration

Slide Type
Sub-Slide
Talk about some of the relationships you observed in this part of the investigation. Were there features that strengthened each other in terms of looking at your feature(s) of interest?
-I decided to study further the relationship between age,weight on one side and the body type on the other side which gave a logical result of Most of the younger players have less weighs and more of a lean body type.

Were there any interesting or surprising interactions between features?
The increase of value of player within suitable age margin results in higher work rate.This show the impact of the reward on the performance



**Key Insights for the presentation:**

I looked further into AGE, to see what other relationship or influence it has with other variables like Weight, Work rate, Body type and Acceleration. I used Facet plot and Heat map to note these findings. Most of the younger players weighs lesser and they also have more of a lean body type. Players whose work rate is High/High, High/Medium have a high acceleration and the Low/Low have a lower acceleration.
