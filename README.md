# Project1-Happiness-Correlations
Prime Country Candidates For Investment and Travel

### Project Description/Outline:
For Project 1, you will work with your group to find and analyze a dataset of your choice. 

 
### Research Questions to Answer:
1. Is there a correlation between Happiness and Safety?<br>
2. Is there a correlation between Happiness and Cost of Living?<br>
3. Is there a correlation between Happiness and Purchasing Power?<br>
4. Which countries satisfy the priorities of the customer best-- does the customer value happiness, purchasing power, or safety most?<br>
5. Which countries on the priority lists have the most developed infrastructure using GDP as a proxy for infrastructure development?<br>


#### Collaborators:<br>
Karoly Burgyan<br>
Shayla Badeaux<br>
Christian Cantu


#### Sources:
1.	World Happiness Report up to 2022. (2022, March 19). Kaggle. https://www.kaggle.com/datasets/mathurinache/world-happiness-report
2.	Cost of Living Index 2022. (2022, May 28). Kaggle. https://www.kaggle.com/datasets/ankanhore545/cost-of-living-index-2022
3.	World Crime Index. (2022, November 8). Kaggle. https://www.kaggle.com/datasets/ahmadjalalmasood123/world-crime-index
4.	AI Global Index. (2023, April 26). Kaggle. https://www.kaggle.com/datasets/katerynameleshenko/ai-index
5.	Stack Overflow - Where Developers Learn, Share, & Build Careers. (n.d.). Stack Overflow. https://stackoverflow.com/
6.	https://chat.openai.com/: used to help debug problematic code

### Analysis:<br>
Datasets for happiness, cost of living (which included purchasing power), and crime (safety) were merged together producing one large merged dataset.

The safety index across each country was stated by city and so, to get a rough estimation of the country-wide safety index, the safety index across all the cities in a country were combined into an averaged for the country.

The statistical outliers of the merged dataset for the values of happiness, cost of living, purchasing power, and safety were attributed to error in measurement and were removed from the dataset.

Correlations between happiness and safety, happiness and cost of living, and happiness and purchasing power were calculated using linear regressions. These correlations were 0.35, 0.74, and 0.74 respectively.

Because purchasing power had the same correlation to happiness as cost of living and it has more salience in terms of investing from the perspective of real estate companies and travel agencies, the cost of living was determined to be less useful and perhaps redundant in the presence of purchasing power.

Z-scores were calculated for the happiness, safety, and purchasing power to assess whether the values varied sufficiently to assess the importance of each metric. If the z-scores were small (eg less than 1 standard deviation) for a metric, then it could be assumed that the metric was less relevant in comparison to the other two metrics.

3D plots were created to visualize the z-scores and assess their variability. It turned out that all three metrics varied well beyond 1 standard deviation and, thereby, suggesting that each metric represented a tangible difference across the countries that shouldn't be discarded.

From the 3 metrics happiness, safety, and purchasing power, the following 7 different prioritization combinations were considered and a histogram for each prioritization was created:
  i. Equally weighted happiness, safety, and purchasing power
  ii. Prioritized happiness, safety, then purchasing power
  iii. Prioritized happiness, purchasing power, then safety
  iv. Prioritized safety, happiness, then purchasing power
  v. Prioritized safety, purchasing power, then happiness
  vi. Prioritized purchasing power, safety, then happiness
  vii. Prioritized purchasing power, happiness, then safety

From those 7 prioritizations, a total of 17 unique countries were collected.

A new dataset of Gross Domestic Product by country by year was introduced as a proxy for a comparison of growth of infrastructure among the 17 unique countries.

A line plot showing the last 5 years of the top 17 countries revealed that top 5 growing countries were Saudi Arabia, Israel, Slovenia, United Arab Emirates, and Austria.
