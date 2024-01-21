# NBA Regression
## Summary
The main purpose of this study was to determine which on-court stats are the most influential to winning basketball games and by doing so, use these variables to make predictions on team performance. Many theories on the matter exist, for example some older theories claim that defense is most influential. Conversely, modern theories claim that 3 point shooting is most important. This study concluded that there is merit to both aforementioned theories and the most influential on court stats are: field goal %, 3 point %, offensive rebounds, defensive rebounds, assists, blocks, steals, turnovers, and personal fouls. The statistical method used was multiple linear regression and the fit criteria used was the AIC. Final regression coefficient output: 
![image](https://github.com/kaven611/NBA_Regression/assets/156690481/0467a495-80ca-4ee8-b91b-68e17896fc6a)

 ## Data Acquisition
 The data used in this study was gathered from https://www.basketball-reference.com. This site has a plethora of different NBA stats and allows you to download as a CSV file.

 ## Data Preparation
 Since basketball-reference.com posts the data on a per season basis each CSV I downloaded only contained one season. I wanted 15 seasons in order to have a large enough data set to separate it into a train and test set. However, I did not want to include any seasons beyond 20 years old as these may skew the data. For example, many rules have changed over the years, affecting the gameplay and therefore the stats.

In terms of data cleaning, there were no missing or incomplete values. All the data was numeric except for team name and season. Since the season crosses over January the season was a string like "2002-2003". Since I was not performing any time series analysis I left this variable as is.

## Data Analytics
