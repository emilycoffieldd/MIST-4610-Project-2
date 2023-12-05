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

When looking at contributing factors to suicide, it might be helpful to examine demographics that are more succeptable to mental health problems. What races struggle more? Does gender play a role? What about ethnicity? Similar to question 1, the analysis and results from question 2 can help with targeted prevention measures and new policy developments. However, it specifically dives into cultural and social sensitivity as it takes into account how different demographic groups can have differing cultural perspectives on suicide, which is a crucial part of the research considering how a lack of cultural sensitivity in the preventive measures can potentially backfire. Furthermore, analyzing different demographic factors and their impact on suicide rates can lead to deeper research into mental health disparities among the different groups as well.


# Data Manipulations

### Have suicide rates gone up over time?

The data for this question has not been altered or adapted.

### What sort of demographic factors impact suicide the most?

Our team created a ‘Race’ calculated field, the likes of which were calculated from information taken from the ‘Stub Label’ column to differentiate by race in a more concise way than the data was originally presented. ‘Sex’ was a calculated field created to differentiate by sex (‘Female’ or ‘Male’) in a way that is separated from race entirely, hence allowing the data to be more bianary and more simplified for the sake of the question. ‘Hispanic’ is our last calculated field, and it was drafted to differentiate between Hispanic Origin, or lack thereof for the ease of modeling.


# Analysis and Results

### Have suicide rates gone up over time?

![image](https://github.com/emilycoffieldd/MIST-4610-Project-2/assets/148081148/a2d7bbef-89ce-486b-99b2-2b689969b24e)


Overall, the total population graph indicates a slight increase in suicide rates over time, with some fluctuations but no abrupt shifts observed. The trend remained relatively stable until around the 2000s, after which there was a more noticeable upward trend. To analyze if there were any possible contributing factors, we compared various graphs filtered with the different demographic factors (age, sex & race) to see if any of them made a huge impact specifically during the shift (1986-2018). 

![image](https://github.com/emilycoffieldd/MIST-4610-Project-2/assets/148081148/e5787a67-393b-431a-9a78-043577256ab1)

The suicide rates during the shift (1986-2018) are then broken down by various age groups.  Based on this graph, we can infer that different age groups illustrate different trends: 
Although the 15-24 years and 25-34 years age groups appear to have lower rates than any other age groups, they exhibit fluctuations over time. Middle-aged groups (35-44 years, 45-64 years) show higher rates, with a particular increase in the last part of the time series, suggesting a growing mental health concern in these demographics. The oldest group (65 years and older) also have higher rates, but the trend seems to be more stable compared to the middle-aged groups, so this can potentially just be an environmental response the suicide in general seeing an uptick.

The last two graphs depict suicide rates from 1986 to 2018, broken down by race for both females and males. In a general picture, the suicide rates among females have increased over time for all racial groups. However, the rates vary by race. The graph does show some abrupt shifts, particularly a sharp increase in the rate for one group around the late 2010s. White females have a notable upward trend, showing higher suicide rates than other racial groups throughout the period, and the rates seem to increase more sharply towards the end of the timeframe, while American Indian or Alaska Native females exhibit a significant spike in suicide rates towards the late 2010s. The rates for Black or African American, and Asian or Pacific Islander females remain relatively lower compared to the other groups, but there's still a visible increase over the years. Hispanic or Latina females show a moderate increase, with rates lower than White females but higher than Black or African American, and Asian or Pacific Islander groups.

Referencing the second half of the visual again, male suicide rates are higher than female rates and show a clear upward trend. There has been a dramatic increase in suicide rates for American Indian or Alaska Native males in the last few years, showing a very steep rise towards the end of the period, with rates surpassing other groups. White males have the highest suicide rates among all racial groups which is not new information to a lot of Americans, but these rates have escalated significantly in the last few years of the data. Hispanic or Latino, Black or African American, and Asian or Pacific Islander males have lower suicide rates compared to White and American Indian or Alaska Native males. However, there's an upward trend observed in these groups too, especially in the last decade.

Overall, based on these observations, we can try to fully understand the contributing factors by making correlations between these trends with other societal and economic data points during the same periods. The possible contributing factors in suicide rates among the middle-aged groups could include age-specific issues such as developmental challenges in younger groups, possibly economic or existential issues in middle-aged groups, and health-related or social isolation issues in the older age groups. The possible contributing factors to the increase in female suicide rates may include socioeconomic conditions, access to mental health care, differing female roles/rights in each culture, and possibly the impact of social media or other recent societal changes no, which could have different impacts across racial female groups. The possible contributing factors for the increase in male suicide rates might include economic stressors, societal pressures, masculinity norms, substance abuse, and mental health issues, which can affect racial groups differently. In a general sense, Americans who commit suicide might be influenced by a rapidly expanding media that may perpetuate feelings of hopelessness and loneliness, an underdeveloped mental health system in America coupled with the stigma around recieving such help, and evolvinhg attitudes in existence like nihilism that tempt victims into this mindset.


### What sort of demographic factors impact suicide the most?

*

# Tableau Packaged Workbook

*
