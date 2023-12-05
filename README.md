# MIST-4610-Project-2

# 29704 Group 6

Luis Garcia @LuisCVG - https://github.com/LuisCVG/MIST-4610-Project-2.git

Emily Coffield @emilycoffieldd - https://github.com/emilycoffieldd/MIST-4610-Project-2.git 

Efe Guvenc @eguvenc03 - https://github.com/eguvenc03/EG-MIST-GroupProjectTwo

Eris Jang @erissjang - https://github.com/erisjang/MIST-Project-2

Jessica Nguyen @jessngph09 - https://github.com/jessngph09/MIST4610-Project2

# Dataset Information

Our team set out to use a data file from the US Data gov website (https://catalog.data.gov/dataset). We examined the different datasets and sought out one that we could use to accurately model two questions about American society and culture. These questions would hold some sort of public and predictive significance when modeled. In saying that, we chose a data set that examined the demographics of Americans of people who committed suicide overtime (i.e. race, sex, age, etc.) The data set we selected has more than 6000 rows of data as well as 13 columns.

Some of the important columns to note are the "ESTIMATE", a decimal, column that numbers the persons in a given population of 100,000 who committed suicide, "STUB_NAME_NUM" and "STUB_LABEL_NUM", an integer and a decimal respectively assigned to distinct stubs, which identify the "STUB_LABEL", a varchar data type, column- which is a column that denotes the demographics of the population. "AGE", a range denoted by a varchar, is another important column that denotes the age of the population being monitored and is distinguished by the identifying column "AGE_NUM", a unique decimal assigned to each distinct age range. Finally, "YEAR", a datetime, is possibly our most important column in the set as it distinguishes the year that the measure was collected in. 

# What We Want to Find Out

### Have suicide rates gone up over time?

We wanted to examine the trend of suicide rates overtime. Have they gone up? Are their any points of abrupt uptick? This might highlight some contributing factors. Being able to read the suicide rate trend throughout the years is crucial as it allows one to visit a few concerns and develop suicide prevention strategies. The identification of the abrupt shifts in the trend allows one to revisit the possible contributing factors such as major historical events at the time, economic factors, sex, etc. In addition, the analysis of the contributing factors can lead to interventions for specific populations or the development of new policies.  Furthermore, the advocation for mental health and the increase in community support can be more heavily enforced during times when there are similar contributing factors reappearing in the future. 

### What sort of demographic factors impact suicide the most?

When looking at contributing factors to suicide, it might be helpful to examine demographics that are more susceptible to mental health problems. What races struggle more? Does gender play a role? What about ethnicity? Similar to question 1, the analysis and results from question 2 can help with targeted prevention measures and new policy developments. However, it specifically dives into cultural and social sensitivity as it takes into account how different demographic groups can have differing cultural perspectives on suicide, which is a crucial part of the research considering how a lack of cultural sensitivity in the preventive measures can potentially backfire. Furthermore, analyzing different demographic factors and their impact on suicide rates can lead to deeper research into mental health disparities among the different groups as well.


# Data Manipulations

### Have suicide rates gone up over time?

The data for this question has not been altered or adapted.

### What sort of demographic factors impact suicide the most?

Our team created a ‘Race’ calculated field, the likes of which were calculated from information taken from the ‘Stub Label’ column to differentiate by race in a more concise way than the data was originally presented. ‘Sex’ was a calculated field created to differentiate by sex (‘Female’ or ‘Male’) in a way that is separated from race entirely, hence allowing the data to be more binary and more simplified for the sake of the question. ‘Hispanic’ is our last calculated field, and it was drafted to differentiate between Hispanic Origin, or lack thereof for the ease of modeling.


# Analysis and Results

### Have suicide rates gone up over time?

![image](https://github.com/emilycoffieldd/MIST-4610-Project-2/assets/148081148/a2d7bbef-89ce-486b-99b2-2b689969b24e)


Overall, the total population graph indicates a slight increase in suicide rates over time, with some fluctuations but no abrupt shifts observed. The trend remained relatively stable until around the 2000s, after which there was a more noticeable upward trend. To analyze if there were any possible contributing factors, we compared various graphs filtered with the different demographic factors (age, sex & race) to see if any of them made a huge impact specifically during the shift (1986-2018). 

![image](https://github.com/emilycoffieldd/MIST-4610-Project-2/assets/148081148/e5787a67-393b-431a-9a78-043577256ab1)

The suicide rates during the shift (1986-2018) are then broken down by various age groups.  Based on this graph, we can infer that different age groups illustrate different trends: 
Although the 15-24 years and 25-34 years age groups appear to have lower rates than any other age groups, they exhibit fluctuations over time. Middle-aged groups (35-44 years, 45-64 years) show higher rates, with a particular increase in the last part of the time series, suggesting a growing mental health concern in these demographics. The oldest group (65 years and older) also have higher rates, but the trend seems to be more stable compared to the middle-aged groups, so this can potentially just be an environmental response the suicide in general seeing an uptick.

The last two graphs depict suicide rates from 1986 to 2018, broken down by race for both females and males. In a general picture, the suicide rates among females have increased over time for all racial groups. However, the rates vary by race. The graph does show some abrupt shifts, particularly a sharp increase in the rate for one group around the late 2010s. White females have a notable upward trend, showing higher suicide rates than other racial groups throughout the period, and the rates seem to increase more sharply towards the end of the timeframe, while American Indian or Alaska Native females exhibit a significant spike in suicide rates towards the late 2010s. The rates for Black or African American, and Asian or Pacific Islander females remain relatively lower compared to the other groups, but there's still a visible increase over the years. Hispanic or Latina females show a moderate increase, with rates lower than White females but higher than Black or African American, and Asian or Pacific Islander groups.

Referencing the second half of the visual again, male suicide rates are higher than female rates and show a clear upward trend. There has been a dramatic increase in suicide rates for American Indian or Alaska Native males in the last few years, showing a very steep rise towards the end of the period, with rates surpassing other groups. White males have the highest suicide rates among all racial groups which is not new information to a lot of Americans, but these rates have escalated significantly in the last few years of the data. Hispanic or Latino, Black or African American, and Asian or Pacific Islander males have lower suicide rates compared to White and American Indian or Alaska Native males. However, there's an upward trend observed in these groups too, especially in the last decade.

Overall, based on these observations, we can try to fully understand the contributing factors by making correlations between these trends with other societal and economic data points during the same periods. The possible contributing factors in suicide rates among the middle-aged groups could include age-specific issues such as developmental challenges in younger groups, possibly economic or existential issues in middle-aged groups, and health-related or social isolation issues in the older age groups. The possible contributing factors to the increase in female suicide rates may include socioeconomic conditions, access to mental health care, differing female roles/rights in each culture, and possibly the impact of social media or other recent societal changes no, which could have different impacts across racial female groups. The possible contributing factors for the increase in male suicide rates might include economic stressors, societal pressures, masculinity norms, substance abuse, and mental health issues, which can affect racial groups differently. In a general sense, Americans who commit suicide might be influenced by a rapidly expanding media that may perpetuate feelings of hopelessness and loneliness, an underdeveloped mental health system in America coupled with the stigma around receiving such help, and evolving attitudes in existence like nihilism that tempt victims into this mindset.


### What sort of demographic factors impact suicide the most?

![image](https://github.com/emilycoffieldd/MIST-4610-Project-2/assets/148081148/bad60ec2-60f6-4705-8c84-4e81dcb78738)

First looking at suicide rates on the basis of sex, it is important to understand this is reference to sex within a biological binary, not gender, which shapes our findings. Taking a look at the comparison of Suicide Rates, on a yearly basis, for Males vs. Females, one can observe that Females- colorized in pink- have shown lower rates on a consistent basis than males- colorized in blue- who make up a larger area of the graph above, hence taking up a higher proportion of the population suicide rate with data spanning from 1950 to 2018. The conversation regarding the gap in men's mental health is nothing new, but why is this? Social trends might point to the fact that men do not have as many close intimate friendships as women, that there is a stigma around men seeking mental health help, that men experience a higher sense of hopelessness socially. On a closer, analytical level, we see a slight dip followed by a rise between the time period of 1990 to 2010. Researchers may use this data to allocate more time looking into social events, politics, socio-technological advances, and/or other factors during the turn of the century. For example, could 9/11/01 have had an impact on the following rise of rates? Maybe the influx of social media? The recession? The further analysis of the time period is crucial.

![image](https://github.com/emilycoffieldd/MIST-4610-Project-2/assets/148081148/9db510d4-f582-4968-bbc3-7cbe0a08a192)

We took our research into the filter of race next. Comparing Suicide Rates, on a yearly basis, can yield a pretty complex output, likely due to the complexity and nuance of the concept of race itself. Taking a closer look at some evident trends in the data, we can observe the highest rate of suicide for ‘White’ (green) people, ‘American Indian’ (blue) in second, followed by a cross of ‘Asian or Pacific Islander’ (orange) and ‘Black or African American' (red). This data is likely not indicative of attitudes regarding suicide for the racial groups that are statistically more apt to it, but rather the attitudes of those lessapt, suggesting potential for a cultural taboo regarding the act.Taking a closer look at the criss-cross of Asian and African American, one can see that starting in 2001, the rates upon African Americans exceeded that of Asians. What may have been the reason behind this? Researchers may once again target social events and cultural ideologies to examine causes. Massive spikes occurred for American Indian and Black citizens during 1985, what may be the cause? The Civil Rights era was a pivotal movement in the history of our country. With ups and downs, could an indirect impact have been the rise of minority suicide cases?

![image](https://github.com/emilycoffieldd/MIST-4610-Project-2/assets/148081148/c0996564-e575-4bbe-99e8-bba15ce7df3f)

Our data only has data on ethnicity in the binary of hispanic and non-hispanic, but it is important to recognize that America is a blend of many ethnicities not represented by this particular data set. However, as a major ethnic group, this data is useful in allowing researchers to examine the rates among Latino-Americans. Taking a closer look at whether classification of ‘Hispanic or Latino’, shown in red, impacts suicide rates is observed above. For individuals that are NOT Hispanic or Latino, shown in blue, a massive increase may be observed starting in 1998 and continuing to rise at a steady pace thereon. What may be the cause? Referring to social events may be the best way to go about this reasoning. Particularly looking at events that impacted races excluding those self-classifying under ‘Hispanic or Latino’. Observably, 'Hispanic or Latino' suicide rates are relatively low and stable which could indicate a cultural taboo regarding suicide.

![image](https://github.com/emilycoffieldd/MIST-4610-Project-2/assets/148081148/23470e7f-0d48-4f56-a5b8-c17cc248c5d0)
![image](https://github.com/emilycoffieldd/MIST-4610-Project-2/assets/148081148/3ce59100-722d-40be-9f1d-2d0b3c6d1b6a)
![image](https://github.com/emilycoffieldd/MIST-4610-Project-2/assets/148081148/bc47978e-9fc7-4988-b1f1-265e96c71864)


Referencing age in this final diagram, it is observable that people later in life used to have higher suicide rates, which can probably be traced to end-of-life suicides as well as other factors. However, as life expectancy rises, those in the '65 Years or Older' catergory begin to experience rates which could conceivably be caused by this age range's population total increasing as end-of-life suicides are dilluted by a growing class of boomers. Meanwhile, suicide rates at '45-64 Years' have only gone up which is more likely to be a concern of mental health attitudes that might be attributed to mid-life hopelessness and a "dead-end mentality". Finally, it is important to observe that suicide rates for those ages '15-24 Years', while being the lowest, have experienced the greatest rate of change over time, rapidly approaching rates of those over the age of 65. It is abundantly possible that this could be caused by the age of the internet as younger generations are the most likely to participate in social media and other forms of technological entertainment that might bring to light attitudes of hopelessness and humiliation in ways older Americans have never before experienced.

In reference to all these findings, we can begin to put together a profile of what someone who is tempted by suicide might look like. They may be male, may be White or American Indian, likely to be ethnically non-Hispanic or Latino, possibly middle-aged. A profile like this can indicate approximately which groups are struggling with mental health most and how extremely. When a person can be statistically identified, they can be researched, allowing scientists and mental health professionals pinpoint how best to help these people who are experiencing this particular flavor of hopelessness. In regards to sex, clearly men have a higher disposition to suicide, so what emotionally affirming services can be marketed to them? White Americans and American Indians also experience significantly higher suicide rates than their AAPI and Black American counter parts, especially those of non-Hispanic or Latino origin, so what can be done to shift the attitudes in these groups of people? Finally, our data can kickstart initiatives that target specific age demographics in intentional ways. For example, researchers might target young adults with cyber-bullying check-ins, older adults with anti-loneliness initiatives. Finding the profile on an American who is statistically more likely to commit suicide and why is the first step in combatting rising suicide rates.

# Tableau Packaged Workbook
### Have suicide rates gone up over time?

[Workbook 1](https://github.com/emilycoffieldd/MIST-4610-Project-2/blob/main/MIST%204610_Project%202_Question%201.twb)

### What sort of demographic factors impact suicide the most?

[Workbook 2](https://github.com/emilycoffieldd/MIST-4610-Project-2/blob/main/U.S.%20Rates%20of%20Suicide%20Over%20time.twbx)
