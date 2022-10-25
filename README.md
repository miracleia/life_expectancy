# An Analysis of Life Expectancy and its Predictive Variables between 2000 and 2015
## by Miracle I. Abraham


## Dataset

This project explores data from Life Expectancy variables extracted from the World Health Organization's [Global Health Observatory](https://www.who.int/data/gho)(GHO) repository. The GHO tracks 20 demography-dependent, critical, and representative health-related factors for 193 countries between the years 2000 and 2015. </br>

This version of the dataset was obtained from a [Kaggle repository](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who) made available by [Kumar Rajarshi](https://www.kaggle.com/kumarajarshi). In the earlier collection and cleaning process, the data had been extracted and combined from multiple sources in the GHO repository. However, I wrangled the data in 4 steps to ensure maximal quality and tidiness for my analysis. These steps are:

1. Renaming the columns to remove leading and trailing whitespaces, make all names lowercase, and replace all spaces with underscores.
2. Dealing with null values by dropping unneeded columns with high numbers of null values as well as all rows with null life expectancy.
3. Dropping other unneeded fields from the dataset.
4. Converting the `Status` column to a dummy variable with the value 0 to represent a developing country and 1 for a developed one.

## Summary of Findings

> My analysis showed a much higher population of developed countries, with 32 developed countries and 151 developing ones in the dataset. For the entire dataset, life expectancies between 60 to 80 years were most common. When separated, the median expectancy for developing countries was about 70 years while developed countries had a median life expectancy of about 80 years.

> High rates of infant death and measles occurrences were quite uncommon in the general dataset, as was high alcohol consumption, though at a much lower degree. All the outlier rates of infant death above 1000 infants per 100,000, were found to be from India. This exception served as an indicator to the country's average life expectancy that fell years below the average trend for every year between 2000 and 2015.

> Most countries appeared to have spent between 5 - 10% of their total annual expenditure on health, but very few countries had this health expenditure surpass 5000% of their GDP per capita. Total expenditure had a moderately high correlation with life expectancy, but the percentage expenditure and GDP had much stronger correlations, suggesting an increasing order of importance in determining life expectancy. True to the strong correlation, countries with health expenditure of more than 10,000% of the GDP per capita consistently had life expectancy greater than other countries by at least 10 years.

> Japan, Sweden, Iceland, Switzerland and France had the highest average life expectancy between 2000 and 2015, while Sierra Leone, Central African Republic, Lesotho, Angola, and Malawi had the lowest average expectancies. 

> Canada, Chile, Finland, France, Greece, Israel, and the Republic of Korea are developing countries with life expectancies greater than 80 years, with most of them being between 81 and 83 years. True to their high life expectancy, all of these countries have less than 100 adults dying per 1000 people, and a maximum of 3 infant deaths per 100,000 children.
While all of these countries have GDPs per capita no higher than 60,000USD, their percentage expenditure on health per GDP is surprisingly moderate as well. However they have low alcohol consumption, measles occurrences, as well as high overall years of schooling and rates of immunization against diphtheria and polio.

> There is a sharp difference in the correlation between life expectancy and Body Mass Index(BMI) for developing and developed countries. BMI and life expectancy have a strong positive correlation for developing countries, but the general expectancy remains lower than the developed countries which, on the other hand, have a weak negative correlation with BMI. The difference between life expectancy for both groups is most obvious for countries with low BMI, while those with higher BMI are more similar.


## Key Insights for Presentation

> Select one or two main threads from your exploration to polish up for your presentation. Note any changes in design from your exploration step here.

1. Interaction of infant death with life expectancy
2. Difference between Life Expectancy-BMI correlation for developing and developed countries.