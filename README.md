# data-512-project

### Basic Overview
Over the last few years, covid has impacted a lot of lives across the globe and a lot of research has already been done to understand the trends and forecast how the infection will spread in future. In this repository I have analysed the covid data about confirmed cases, mask mandate rules and how these rules impacted the infection. The analysis is only done for Allegheny County,	Pennsylvania in this repository.

## Files Description

#### Input Data
1) RAW_us_confirmed_cases.csv file from Kaggle repository [source - https://www.kaggle.com/datasets/antgoldbloom/covid19-data-from-john-hopkins-university]
2) RAW_us_deaths.csv file from Kaggle repository [source - https://www.kaggle.com/datasets/antgoldbloom/covid19-data-from-john-hopkins-university]
3) mask-use-by-county.csv from New York Times [source - https://github.com/nytimes/covid-19-data/tree/master/mask-use]

Other data used
1) U.S._State_and_Territorial_Public_Mask_Mandates_From_April_10__2020_through_August_15__2021_by_County_by_Day.csv [source - https://data.cdc.gov/Policy-Surveillance/U-S-State-and-Territorial-Public-Mask-Mandates-Fro/62d6-pm5i]


#### Output Plots
1) masking_policy_vs_confirmed_cases.jpeg - Displaying masking policy over time along with number of confirmed cases at a daily level
2) masking_policy_vs_infection_rate.jpeg - Displaying masking policy over time and its impact on the change in rate of infection


## Notebook - data512_CommonAnalysis.ipynb
The notebook is well documented  and is broadly divided into 4 section. 
* Section 1 - The first section involves installing libraries and loading the data.

* Section 2 - This section focuses on extracting information only for the required county (Allegheny County,	Pennsylvania). The extracted data from the data files is merged to create one dataframe. 

 * Section 3 - The third part of this notebook involves performing basic data analysis to understand the trends. 
 * Section 4 - Finally a visualization is generated to display how masking mandate were changed over time and how this impacted the confirmed cases and infection. 

## Dependencies and installation
Apart from pre-installed libraries from anaconda, this notebook uses a library called Ruptures. Here is instruction to installation.
 !pip install ruptures
 
 
## Conclusion and Reflection
The final results and conclusion are included in the repository as pdf. Additionally informaiton about collaboration with other colleagues working on data analysis for other county across the United States as pdf file.

## References
- Rate of infection calculation - https://en.wikipedia.org/wiki/Infection_rate
- Concept of change points - https://medium.com/dataman-in-ai/finding-the-change-points-in-a-time-series-95a308207012
