<!DOCTYPE html>
<html>
<head>

</head>
<body>
<h1>Data Clean-Up:</h1>
<p>1. First, we imported all our dependencies, and saved the path to the CSV file as a new variable. Then, using that variable, we could read the CSV file into a dataframe. Using the df.info() function, we are able to determine if there were any non-null values (none), and the dtypes of each column. Because this call returned no non-null types and no NaN values, we determined our dataframe to be clean, without any values missing or irrelevant. Therefore we were able to use this dataframe as a good starting point to begin filtering for the appropriate data.</p>
<p>2. We decided to use the same Jupyter Notebook for our data analysis because the clean-up process was not as intensive.</p>
<hr>
<h2>General Questions:</h2>
<ol>
<li>In the US, are there any discernible trends over the years for the number of births?</li>
<li>What about the weight of the baby? Can factors such as the age of the mother or her education level affect her baby's weight?</li>
<li>Is there a trend between gender and weight? Does the state a mother is living in have any effect on her baby's weight?</li>
</ol>
<hr>
<h2>Analyses:</h2>
<h3>1. Number of Births Per State [Hannah]:</h3>
<p>a. It can be inferred from this data set that the states with the largest populations are the states that have the highest birth rates. California, Texas and Florida are the most densely populated states, and thus have the highest birth rates. The land mass of the state does not always determine the size of the birth rate, as some states such as Alaska and Wyoming have large land masses, but lower birth rates that more heavily populated states such as California.</p>
<p>b. I had gone into this data set believing that the more conservative states would have the highest birthrates, but that is not necessarily true. Wyoming is one of the most conservative states, but has one of the lower birth rates. Similarly, California is a very liberal state and has the highest birth rates.</p>
<h3>2. Number of Births Per Gender Per State [Christina]:</h3>
<p>a. The number of births varied across different states, with some states having higher birth rates than others. There are many factors that can affect population dynamics, such as social and economic factors. It can help researchers and analysts study the correlation between birth rates and several socio-economic factors, such as income levels, education, employment, and cultural factors.</p>
<p>b. This information can help to better understand areas such as education, labor market planning, and social welfare programs. Understanding the distribution of births per state can help public health officials in planning and allocating resources, such as healthcare facilities and services, to meet the needs of the population. States with higher birth rates might require additional support to ensure proper healthcare for mothers and infants is provided.</p>
<p>c. In conclusion, the analysis of the number of births per state per gender provides valuable information for population dynamics and potential factors influencing birth rates. The data can inform public health planning, social and economic analysis, and resource allocation decisions, leading to more effective resources for maternal and child welfare.</p>
<h3>3. Average Birth Weight (g) Per State (Are there any states with average under or overweight babies?) [Steph]:</h3>
<p>a. We decided to go with a bar chart for this type of analysis, and sorted the mean values from least to greatest, with the average baby weight of Mississippi being the lowest and Alaska being the highest.</p>
<p>b. If we look at just these two states geographically, they are in extremely different parts of the US, and this might affect a baby's weight: Alaska is in the extreme northern part where families might place more of an emphasis on staying warm and therefore not exposing their babies to the outside, while Mississippi is prone to heat and humidity.</p>
<p>c. We might also consider the relative family income of each state and if there is any impact on baby weight. For example, states like California and New York are among those with the highest family incomes, while states like Georgia and Alabama are not. However, we were not able to find any datasets that matched or overlapped the years with which our main dataset was based on, and so this must still be considered speculation.</p>
<p>d. Another factor we could consider is a mother's access to healthy food that might affect her baby's weight; we could look at where these women were living at the time of birth and look at the surrounding area for supermarkets (with fresh foods) and/or fast food places. But because of the way the dataset is set up (the dataframe is grouped by education level of the mother with the number of births per education level), we were unable to gather this. We would also need the addresses of each subject which is clearly out of this dataset's scope.</p>
<p>e. We are able to determine that all states' average baby weights fall between the healthy range of 5lbs, 8oz (2500g) and 8lbs, 13oz (4000g), so we can conclude that no states have average under or over baby weights.</p>
<p>f. We have also calculated the standard deviation for these values and this came out to be 48.88. Because this is a relatively low standard deviation, we can conclude that most of our values are clustered around the mean average baby weight for all states (3250.98g).</p>
<h3>4. Average Birth Weight (g) Per Average Age of the Mother [Nasr]:</h3>
<p>a. After analyzing our recent observations between the Average Age of Mothers and the Average weight of their babies, A line graph was created based on this data. In this graph, there is a pretty visible trend that occurs when we compare these 2 sets of data. As the Average Age of Mother increases the Average Birth Weight of their children also tends to increase.</p>
<p>b. There is a positive trend relationship that could be identified by looking at how each set of data affects each other. Mothers between the ages of 28-29 start to produce on average heavier babies than mothers who are between 23-28. This was interesting because it was the first noticeable spike that we can identify as significant. This could be a result of external factors that this dataset alone does not fully explain. These factors could be a result of hormonal declines or other health factors that are not observed in this dataset.</p>
<p>c. The most significant point of data in this graph is when mothers are between the ages of 29-35. We not only can see a peak in our relationship but also a significant decline shortly after. Babies were, on average, at their heaviest when mothers were at the age of 32, and birth weight experienced a noticeable decline when mothers were between the ages of 32-34. This could be merely a coincidence, or potentially external factors related to health affecting the dataset.</p>
<h3>5. Average Baby Weight Per Gender [Ethan]:</h3>
<p>a. After analyzing the data and visualizing the average weight per gender, several conclusions can be drawn: There is a clear distinction in the average birth weight between males and females. The visualization shows that males tend to have a higher average birth weight compared to females.</p>
<p>b. The difference in average birth weight between genders is noticeable and statistically significant. This suggests that gender plays a role in determining birth weight. The average birth weight for females is around 3194.57 grams (7.04 pounds), while for males, it is around 3307.15 grams (7.29 pounds).</p>
<p>c. The visualization provides a clear and concise comparison of the average birth weight between genders, making it easy to interpret and understand the differences.</p>
<p>d. The data used for this analysis is based on the available dataset, and it is important to note that birth weight can be influenced by various factors such as genetics, maternal health, and prenatal care, among others.</p>
<p>e. In conclusion, the visualization highlights the difference in average birth weight between males and females, providing valuable insights into the gender-specific variations in birth weight.</p>
<h3>6. Average Baby Weight Per Mother's Education Level [Steph]:</h3>
<p>a. Another observation we can infer from the dataset is the trend between baby weight and the mother's education level. It seems there is a slight increase in baby weight as the mother continues her education; this might be due to the mother's initial weight and age (younger mothers in their teens and twenties might weigh less than older mothers in their thirties), but we do see a slight drop-off in weight when a mother has received a doctorate degree.</p>
<p>b. There are, however, a great number of outliers within the doctorate level of education, which might suggest that women who have children in their later years have extremely varied lifestyles and/or health issues that affect their babies' weight.</p>
<p>c. Further analysis might look for other factors, such as the amount of stress a mother is under during her schooling, her eating habits, and the amount of exercise she commits to.</p>
</div>
</body>
</html>
