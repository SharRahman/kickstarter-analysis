# Kickstarting Theater Plays 

## Overview of Project
The purpose of this analysis is to see the trends on how successful Theater/Play kickstarters were from 2010 to 2017. 
Success being defined as meeting or exceeding the fundraiser goal.   

## Analysis and Challenges
This analysis was performed by taking a data dump of kickstarter data and making the data readable into 2 simple graphs to see.   

### Analysis of Outcomes Based on Launch Date
The first graph(https://github.com/SharRahman/kickstarter-analysis/blob/d0a8bff655beb1398c0b135c55cec1b2f71297e3/Resources/Theater_Outcomes_vs_Launch.png) illustrates how many kickstarter campaigns were successfull monthly, ranging from 2010 to 2017.

### Analysis of Outcomes Based on Goals
The 2nd graph (https://github.com/SharRahman/kickstarter-analysis/blob/d0a8bff655beb1398c0b135c55cec1b2f71297e3/Resources/Outcomes_vs_Goals.png) presents the success vs failure trends at the different levels of funding wanted.

### Challenges and Difficulties Encountered
The challenges that were encountered was related to making the data more readable. 
For example, the launch dates of each project was in Unix epoch time and had to be converted using this formula:
_=(((J2/60)/60)/24)+DATE(1970,1,1) _ where J2 is the kickstarter launch date in unix epoch time

## Results

The first conclusion about the Outcomes based on Launch Date is that kickstarters for any genre of Theater (plays, musicals, and spaces) are more likly to succeed than fail. The second conclusion is that kickstarters started in the month of May has a much better chance of succeeding than any other month.    

Based on the "Kickstarter Plays Outcomes Based on Goal" graph, as kickstarters for plays increase in their goal level they have a higher chance of failing. 
And as their goal decreases in level they have a higher chance of being successful in reaching their goal. 
The best goal level to put your kickstarter at so it has atleast a 50% chance of succeeding is $19,999 or less.    
 
Some limitations of this dataset are that the data is only up till 2017, we are currently in 2022, which means the last 4 years of data is missing.
New trends could effect the outcomes of kickstarters for theater, maybe everybody got scared of COVID and all kickstarters for theaters and plays fail now.
Another limitation is that projects can be funded with different currencies. 100,000 SEK is not the same as $100,000 USD, its more like $9,880 USD. 
When we look at this data we should either convert everything to a constant currency or only filter by USD to make the most accurate decisions.   

We could create a pie chart to see which country has the biggest portion of successful kickstarters. 
If you want to do a theater/play in a country that isn't in the pie chart, maybe take this analysis with a grain of salt as your results could be very different from the results of this dataset.
