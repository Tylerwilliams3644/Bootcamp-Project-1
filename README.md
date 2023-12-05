# Bootcamp-Project-1
Data Cleanup Procedures/Writeup

Crime and Income
National crime statistics pulled from the FBI’s National Incident-Based Reporting System through the Uniform Crime Reporting database. (Excel formatting only available).
1 spreadsheet per criminal offense category (crime against property, person, or society) per year
Each criminal offense category contained 5-12 columns of specific offenses
Files converted to cvs, totaled up to each category offenses, merged across years, then merged across criminal offense categories
Merged with income data on shared column of state for analysis


Employment Data
Data was found from bea.gov
The original data set included 104878 rows and 30 columns
Filtered out the rows to only find the rows that was giving us the number of jobs for each individual state from 2012-2022
Then we combined all the like industries to get a total of 14 different industries (down from 33)
We combined all the values for the grouped industries into one, so we have the sum
Lastly we created charts to see how many jobs were in each state for 2022 in each industry 

Income By State
Data was found from bea.gov
The original data set included 9600 rows × 14 columns
Filtered out the rows to only show income levels 
Further filtered to show only income levels for only the 50 states
Found the average income level for each state and added it to the data frame
Created a chart that will display the change in income level for the desired state from 2012-2022
Created a chart that will display the change in the average income levels from 2012-2022
Lastly, created a chart that compares the selected state to the average of all states

Income by County
Data was found from bea.gov
The original data set included 9425 rows rows and 62 columns.
The data went from the year 1969 to 2022. We only used 2012 - 2022.
The original dataset included states and “county,states” in one column. Each state and county included a row containing “personal income”, “population”, and “per capita personal income.” 
The data was filtered to remove the rows with only states and only include rows where a county was listed.
The data was also filtered to only show the “per capita personal income” to show only the average income.
The data frame was organized to match the column names in the state dataframe listed above.
The data was cleaned to separate the “county,state” by placing the state listed after the comma in its own column.
A national average income was concluded and then compared to three of the most populated counties in the USA, then three of the least populated counties.
Charts were created to visualize that difference.
A t-test was conducted to compare the six mentioned counties and compare income.


Analysis
Income and Crime Hypotheses
H0: There is no direct relationship between income and levels of criminal activity.
H1: As levels of income increase, crime levels will decrease negatively by the same rate.

Income and Crime Findings
H0 and H1 were both proven false. Our analysis found that there was a direct positive correlation between increases in income and crime year-over-year.
A fairly strong positive relationship was found across all criminal offense categories: for crimes against persons (e.g. kidnapping, homicides, assaults) the Pearson correlation was 0.74; for crimes against property (e.g. vandalism, robbery, embezzlement/white collar crime) it was 0.73; even for crimes against society (e.g. animal cruelty, narcotics trafficking) it was 0.60. As income increased, so too did criminal offenses.

Income and Crime Conclusions
Contrary to perhaps popular belief, earning more income within a state did not lead to fewer reported instances of crime. There could be several possible explanations. One, this analysis did not address the distribution of income nor crime across a state’s population. It could be as incomes increased, they were concentrated in a small portion of their state’s population and the same for crime. There could also be additional factors that may be simultaneously driving income growth and crime.

Industry and Income Levels
An overarching theme the data shows is, the state makes the industry’s wealth, not the other way around. For example California and Texas are the richest states and also have the most jobs in all industries. This would also make sense because California and Texas have very large populations.
An interesting, but not surprising, chart is the media chart. California has twice as many media jobs as the next most states, New York and Texas, then it falls to states that have almost no media jobs in comparison. Story of the data is if you want a job in the media industry move to California. 
Q1: How do the number of real estate jobs affect the wealth of a state?
Top State: California, Florida, Georgia, Illinois, New Jersey, New York, North Carolina, Ohio, Pennsylvania, Texas
	A1: The states with the most real estate jobs are well above average when it comes to personal income levels for the whole state. This could be because real estate jobs pay above average and would drive income levels. As well, people invest money into property as their income levels rise.


Counties Population vs Income Hypothesis
H0: Population levels have no correlation to the national income average.
H1: There is a positive correlation between higher income levels and higher population levels within each county.On the flipside, there is also a correlation between lower income levels and lower population levels within each county.

Counties Population vs Income Findings
The hypothesis was proven true for higher populated counties. The income average stayed consistently higher than the national income average.
The hypothesis was proven false for lower populated counties. The income average was inconsistent, sometimes ranging far above or below the national income level within a county.

Counties Population vs Income Conclusions
Higher populated counties tend to have a more consistent level of income following a similar pattern as the national trend, while lower populated counties were inconsistent in income with more dramatic changes and less likely to consistently follow the national trend.
