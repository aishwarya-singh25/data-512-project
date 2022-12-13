# data-512-project

## 1. Basic Overview
Over the last few years, covid has impacted a lot of lives across the globe and a lot of research has already been done to understand the trends and forecast how the infection will spread in future. In this repository I have analysed the covid data about confirmed cases, mask mandate rules and how these rules impacted the infection. The analysis is only done for Allegheny County,	Pennsylvania in this repository.

## 2. Files Description

#### 2.1 Input Data
1) RAW_us_confirmed_cases.csv file from Kaggle repository [source - https://www.kaggle.com/datasets/antgoldbloom/covid19-data-from-john-hopkins-university]
2) RAW_us_deaths.csv file from Kaggle repository [source - https://www.kaggle.com/datasets/antgoldbloom/covid19-data-from-john-hopkins-university]
3) mask-use-by-county.csv from New York Times [source - https://github.com/nytimes/covid-19-data/tree/master/mask-use]
4) AlleghenyCounty_combined - previously cleaned and combined file during common analysis
5) COVID-19_Vaccinations_by_Day_by_County_of_Residence_Current_Health [source - https://data.pa.gov/Covid-19/COVID-19-Vaccinations-by-Day-by-County-of-Residenc/bicw-3gwi]

#### 2.2 Output Plots
Preliminery Analysis
1) masking_policy_vs_confirmed_cases.jpeg - Displaying masking policy over time along with number of confirmed cases at a daily level
2) masking_policy_vs_infection_rate.jpeg - Displaying masking policy over time and its impact on the change in rate of infection
Extended Analysis
1) plot1_changepoint_detection.jpeg - Results of changepoint detection
2) plot2_rate_of_infection_vs_masks.jpeg - Change in rate of infeciton over time with masking policy
3) plot3_rate_of_infection_and_death_vs_masks.jpeg - Showing trends for rate of infection and death over time
4) plot4_confirmed_cases_vs_death.jpeg - Displaying number of cases and death over time
5) plot5_vaccination_trend.jpeg - Displaying count of vaccination on daily-level
6) plot6_partially_and_fully_vaccinated.jpeg - Count of partially and fully vaccinated people
7) plot7_subplot_deathcount_vaccinecount.jpeg - final subplot for presentation


#### 2.3 Notebooks
##### Notebook - data512_CommonAnalysis.ipynb
The notebook is well documented  and is broadly divided into 4 section. 
* Section 1 - The first section involves installing libraries and loading the data.
* Section 2 - This section focuses on extracting information only for the required county (Allegheny County,	Pennsylvania). The extracted data from the data files is merged to create one dataframe. 
 * Section 3 - The third part of this notebook involves performing basic data analysis to understand the trends.
 * Section 4 - Finally a visualization is generated to display how masking mandate were changed over time and how this impacted the confirmed cases and infection. 

##### Notebook - data512_final_analysis.ipynb

 * Section 1 and 2 - The first section involves installing libraries and loading the data.
 * Section 3 - Data Preprocessing for datetime variables and missing values
 * Section 4 - Feature Engineering to create and add new features to the data
 * Section 5 - Data Analysis and generating plots 
 

## 3. Dependencies and Installation
Apart from pre-installed libraries from anaconda, this notebook uses a library called Ruptures. Here is instruction to installation.
 
 
 <code>!pip install ruptures</code>
 
## 4. Conclusion and Reflection
The final results and conclusion are included in the repository as pdf. Additionally informaiton about collaboration with other colleagues working on data analysis for other county across the United States as pdf file.

The final report includes a detailed conclusion of the complete project and talks about the future work adn limitations. The pdf document is avaialble in the repository.

## 5. References
- Rate of infection calculation - https://en.wikipedia.org/wiki/Infection_rate
- Concept of change points - https://medium.com/dataman-in-ai/finding-the-change-points-in-a-time-series-95a308207012
- Research paper on COVID vaccine immunity - https://doi.org/10.1038/d41586-021-02532-4
- Research paper on Global impact of the first year of COVID-19 vaccination - https://www.thelancet.com/journals/laninf/article /PIIS1473-3099(22)00320-6/fulltext
