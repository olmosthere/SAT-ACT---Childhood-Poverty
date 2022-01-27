<h1>Project 1 README</h1>

<h2>Problem Statement</h2>

Poverty and its affects on education have always been a major issue in the United States. This project aims to explore if states that have the highest percentage of children under 18 living in poverty have any correlation between the reported ACT scores of those states from 2017 to 2019. It will also give recommendations on how to increase overall SAT composite scores.

<h2>Background</h2>

The ACT has 4 sections: English, Mathematics, Reading, and Science, with an additional optional writing section ([*source*](https://www.act.org/content/act/en/products-and-services/the-act/scores/understanding-your-scores.html)).

"The poverty rate in U.S. is close to 12%, meaning 1 in 8 Americans live at or below the poverty level.  1 in 6 children in the U.S. are living in poverty.  11 million children, or about 1 in 9 of all children in the U.S., live at 50 percent below the federal poverty line.  37% of children raised in poverty do not finish high school." ([*source*](https://www.childfund.org/Content/NewsDetail/2147489206/))

<h2>Data Dictionary</h2>

|Feature|Type|Dataset|Description|
|---|---|---|---|
|state|*object*|ACT 2017-2019/U.S. Census 2017-2019|The U.S. state to which the data applies.|
|participation|*float*|ACT 2017-2019|The percentage of students who participated in the ACT. Participation may be mandated by state.|
|composite|*float*|ACT 2017-2019|The average composite score across all four areas of the ACT.|
|year|*datetime*|ACT 2017-2019/U.S. Census 2017-2019|The year to which the data applies.|
|child_pov_rate|*float*|U.S. Census 2017-2019|Percentage of minors under age 18 living in poverty. For more info on how the U.S. Census Bureau determines the poverty level, click [here](https://www.census.gov/topics/income-poverty/poverty/guidance/poverty-measures.html)|
|region|*object*|U.S. Census Regions 2010|Which region of the U.S. the state resides in. For more info on how the U.S. Census Bureau breaks up the census regions, click [here](https://www2.census.gov/geo/pdfs/maps-data/maps/reference/us_regdiv.pdf)|
|election_2020|*object*|National Archives 2020 Electoral College Results|Determines whether the majority of the state's electoral college votes went toward the Republican candidate (red) or the Democratic candidate (blue) in the 2020 presidential election. For more info, click [here](https://www.archives.gov/electoral-college/2020)|

<h2>Summary of Analysis</h2>

-The majority of states with the highest participation rates require ACT testing for all students.  Top 5 remained the same for all three years.  

-The states with the lowest participation rates are the smallest states in the country that do not require ACT participation.  It's also interesting to note the states with the least participation in the ACT have less minors living in poverty than the states with the highest participation rates.

-The only state west of the Mississippi that made the top 10 mean composite. score list from 2017-2019 was Colorado in 2018.

-Many of the states with the lowest mean composite scores have 100% participation, which may be why the scores are so low. Think about the difference in approach a student would have if they are taking the test because they have to as opposed to because they need to score well on the ACT to get into the colleges they are interested in. These states also hold some of the highest child poverty level in the country.

-Many states have adopted or moved away from mandatory ACT testing. From what our data shows, it may indicate Colorado and Minnesota may have moved away from the ACT as a requirement after 2017. Missouri and South Carolina may have moved away from the requirement after 2018. Alternatively, Nebraska and Ohio may have adopted the mandate after 2017. It could also mean that although the scores were mandated by state, certain districts may not have been able to test all students.

-It's interesting to note the only two states (Iowa & South Dakota) that had participation rates over 50% and average composite scores above the mean composite scores of our datasets for all three years also had child poverty levels below the mean poverty levels for the same years.

-The states with the highest three year median composite scores are all East Coast states, but we noticed how low the three year median participation rates were for those states (none are above 31%).  This would reinforce our earlier observation that a high participation rates don't add up to a high average composite score, in fact it may be suggesting the opposite.

-Highest 𝜇 composite scores are all East Coast states and we noticed how much higher the childhood poverty rates are in the lowest states and the majority of them had participation rates of 100%!

-As we have noticed throughout the EDA, there is a significant negative correlation between the composite scores and participation rates. There is also a noticeable negative correlation between childhood poverty rates and composite scores, but it's not considered significant. Lastly, there is some positive correlation between childhood poverty rates and participation rates, but it's also not considered significant.

-There seems to be a trend that given any participation rate, the states with higher poverty rates get lower composite scores. This trend seems to be most predominant in the states with 100% participation rates.

-States in the Northeast seem to excel in the average composite scores, but they don't have high participation rates. It seems to be the exact opposite for states in the south. States in the Midwest seem to have the high participation rates and composite scores. This trend seems to apply to states in the West, too, but they also seem to have a grouping with higher participation rates and lower composite scores.

-States with the highest composite scores went blue in the 2020 Presidential Election. Also note the state(s) with the lowest composite scores also went blue, but there were much less of them. The states that went red had the highest frequency of 100% participation rates, but the states that had the highest composite scores with 100% participation went blue. There is a solid group of red states that had greater than 60% participation and a composite score above 20.

<h2>Conclusions & Recommendations</h2>

There is a significant negative correlation between a state's participation rate and their composite score.  If time and money are being allocated in mandating students to take the ACT, states should move away from mandatory testing and divert those resources into community programs designed to combat childhood poverty.  The participation rates for those states will absolutely take a hit, but due to the negative correlation it should help raise the composite scores.

In order to find out the best ways to do this this, we should take a look at the ACT policies of the states in Northeast and explore their policies and procedures.  It also looks like the majority of states that require mandatory ACT testing tended to vote Republican in the 2020 presidential election.  These states should look at the policies of the other states that voted Republican in 2020 but had participation above 60% and composite scores above 21, particularly Iowa and South Dakota.  That way they can still prioritize participation rates but raise how well the students are doing on the ACT which is ultimately what matters.
