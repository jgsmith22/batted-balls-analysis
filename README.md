# batted-balls-analysis
Exploration and analysis of public Major League Baseball data. 

**This was my capstone project to finish off my Bachelors of Science in Data Analytics at Western Governors University**

This project will look into whether or not it’s strictly necessary to rely on the numerous advanced statistics available to a baseball organization or if the simple act of putting the baseball into play during an at bat will increase the number of runs a team will score over the course of a season.  

The solution to determining whether or not batted balls leads to an increase in runs scored will be to use scatter plots to visually see any correlation. By graphing batted balls against runs scored for each team during the 2015 to 2022 seasons with Python I should be able to determine what correlation there is. I will also run linear regression models within Python to get a numerical representation of any correlations. Doing this could give organizations a simpler way to build a team around players who put the ball in play. 

The goal of this project is to use Python to graphically and numerically analyze data obtained from Major League Baseball to provide insight into the best statistics to focus on to increase an organizations chances of winning more baseball games and possibly, championships. Specifically this project will focus on the batted ball and runs scored statistics.  
The objectives for this goal:
  •	Determine any possible correlation between batted balls and runs scored over the course of a season for each team in Major League Baseball. 
    o	The deliverable for this objective will be a report that graphically, through scatter plots, and numerically, through summary tables, that show correlations between batted balls and runs scored over the course of a season for Major League Baseball as a whole. 

The project scope will be to produce a summary for the 2015 to 2022 MLB seasons that shows overall correlation between batted balls and runs scored. This summary will be for the league as a whole and will not be broken down by team. Input will be season data for each MLB team and the output will be both a scatter plot of that data as well as a linear regression model with batted balls as the independent variable and runs scored as the dependent variable. Due to the shortened 2020 season from the COVID-19 pandemic, that season will not be included in this project. 

I will use descriptive statistics to look at statistics for each MLB team in past seasons.  I will then use exploratory data analysis to look at correlations between batted balls and runs scored, ending with a linear regression model between the two. 


My main tool will be Python to extract data from websites and to create linear regression models as well as visualizations. Python has numerous libraries that are designed for data collection (Beautiful Soup), data cleaning (Pandas), and visualization (Matplotlib) and analysis (StatsModels). This will allow me to provide easy to understand graphs and tables. 

The metrics I will use to evaluate statistical significance will be the R-squared value and p-value from the linear regression models. My null hypothesis is that there is no positive correlation between number of batted balls and number of runs scored over the course of a season. My goal will be to disprove that hypothesis and prove that there is positive correlation between number of batted balls and number of runs scored in a season. For the p-value I will use a significance value of α = 0.01 and look for a r-squared value of above 0.7. If the p-value < α and r-squared is > 0.7 I will be able to say I can reject the null hypothesis. 

For both the Baseball Reference and Stahead websites you were able to easily export data to a csv file in Excel. I simply found the teams and seasons I needed run statistics for and exported that information into an Excel csv file. The Baseball Savant Statcast data was a little more difficult. While some of the website had exportable data the Statcast data that contained batted ball information was not exportable in any format. To get around this I was able to create a function to scrape the data from the HTML table using Python’s Beautiful Soup library and then converted each season data into its own csv file. Once all the data was scraped or exported into a csv file I was able to use the Pandas library to combine all of the data sets into one master data frame. 

