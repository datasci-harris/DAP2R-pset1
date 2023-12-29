# Data Skills 2 - R
## Winter Quarter 2024

## Homework 1
## Due: January 18, 2024 before midnight on Gradescope

__Question 1 (40%):__ The two datasets included in the assignment repo are downloaded directly from the BEA.  The file labeled "total" has the total employment per state for the years 2000 and 2017.  The file labeled "by industry" has employment per industry in each of 10 industries per state for the same years.

Load and merge the data into a panel dataframe, with the columns: "state", "year", and one for each of the 10 industries.  Every state-year combination should uniquely identify a row.  No more and no less than 12 columns should remain.  Do any necessary cleaning for the data to be easily usable.

The values should be given as the share of the total employment in that place and time, e.g. if total employment in a place and time was 100, and the employment in one industry was 10, then the value shown for that state-year industry should be 0.1.  The "total" values should not be a part of the final dataframe.  

Output this dataframe to a csv document named "data.csv" and sync it to your homework repo with your code.

__Question 2 (30%):__ Write a function that finds the top states with the highest values of a variable in a given year. That is, this function should take as input 3 parameters: the number of states, the industry, and the year. Use this function to find the states with the top 5 of manufacturing employment in the year 2000, then show how their share of employment in manufacturing changed between 2000 and 2017.  Use a basic plot to display the information. Repeat this via a for loop for the top 10 of farm employment in 2000 and top 15 of information in 2017.

__Question 3 (30%)__ Write a function that plots where a given state is in the distribution of employment shares for a given industry in 2000 and 2017, as well as the distribution of the change in employment shares from 2000 to 2017. This function should take as input 2 parameters: the state and the industry. For each year as well as for the difference, it should plot a histogram of employment shares for that industry, and then include a vertical line for the mean of the overall distribution and a vertical line for the value for the given state. It should be clearly denoted which is the mean and which is that state's value. Note that since the shares here are already in percent terms, the change is just calculated as the difference in shares.
