Data Clean-Up:

1. First, we imported all our dependencies, and saved the path to the CSV file as a new variable. Then, using that variable, we could read the CSV file into a dataframe. Using the df.info() function, we are able to determine if there were any non-null values (none), and the dtypes of each column. Because this call returned no non-null types and no NaN values, we determined our dataframe to be clean, without any values missing or irrelevant. Therefore we were able to use this dataframe as a good starting point to begin filtering for the appropriate data. 

2. We decided to use the same Jupyter Notebook for our data analysis because the clean-up process was not as intensive.

----------

General Questions:
1. In the US, are there any discernible trends over the years for births, given factors such as baby weight and the age of the mother?

2. 

Analyses:

1. Average Birth Weight (g) Per State (Are there any states with average under or overweight babies?) [Steph]:

    a. We decided to go with a bar chart for this type of analysis, and sorted the mean values from least to greatest, with the average baby weight of Mississippi being the lowest and the Alaska being the highest. 

    b. If we look at just these two states geographically, they are in extremely different parts of the US, and this might affect a baby's weight: Alaska is in the extreme northern part where families might place more of an emphasis on staying warm and therefore not exposing their babies to the outside, while in Mississippi is prone to heat and humidity. 

    c. We might also consider the relative family income of each state and if there is any impact on baby weight. For example, states like California and New York are among those with the highest family incomes, while states like Georgia and Alabama are not. However, we were not able to find any datasets that matched or overlapped the years with which our main dataset was based on, and so this must still be considered speculation. 

    d. Another factor we could consider is a mother's access to healthy food that might affect her baby's weight; we could look at where these women were living at the time of birth and look at the surrounding area for supermarkets (with fresh foods) and/or fast food places. But because of the way the dataset is set up (the dataframe is grouped by education level of the mother with the number of births per education level), we were unable to gather this. We would also need the addresses of each subject which is clearly out of this dataset's scope.

    e. We are able to determine that all states' average baby weights fall between the healthy range of 5lbs, 8oz (2500g) and 8lbs, 13oz (4000g), so we can conclude that no states have average under or over baby weights.

    f. We have also calculated the standard deviation for these values and this came out to be 48.88. Because this is a relatively low standard deviation, we can conclude that most of our values are clustered around the mean average baby weight for all states (3250.98g).

2. Number of Births Per State Per Gender [Christina]:

    a. The number of births varied across different states, with some states having significantly higher birth rates than others. This suggests variations in population dynamics and potentially different social and economic factors influencing birth rates. It can help researchers and analysts study the relationship between birth rates and various socio-economic factors, such as income levels, education, employment, and cultural factors. 
    
    b. This knowledge can contribute to a better understanding of societal trends and inform decision-making in areas such as education, labor market planning, and social welfare programs. Understanding the distribution of births per state can assist public health officials in planning and allocating resources, such as healthcare facilities and services, to meet the needs of the population. States with higher birth rates may require additional support and infrastructure to ensure adequate healthcare for mothers and infants.In conclusion, the analysis of the number of births per state per gender provides valuable insights into population dynamics, demographic trends, and potential factors influencing birth rates. The data can inform public health planning, policy development, social and economic analysis, and resource allocation decisions, leading to more effective and targeted interventions for maternal and child welfare.

3. 