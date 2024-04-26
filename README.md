# wine
evaluating different model prediction to classify wine class

### Overview
With a global population growing and the challenges climate change brings, guaranteeing food security becomes a key factor for the stability of any country. Two of the dimensions of [food security](https://www.worldbank.org/en/topic/agriculture/brief/food-security-update/what-is-food-security) are: a) Physical Availability, which is determined by the level of food production, stock levels and net trade, and b) Stability: adequate access to food on a periodic basis, where adverse weather conditions, political instability, or economic factors (unemployment, rising food prices) may have an impact on the food security status. 

Due to the increased amount of extreme weather events and changes in the weather conditions as a consequence of climate change, it is imperative to plan for the future based on predictions that can be established in the present.

The area of study correspond to four countries categorized by [The World Bank](https://datahelpdesk.worldbank.org/knowledgebase/articles/906519-world-bank-country-and-lending-groups) as low-middle income Economies with a Gross National Income (GNI) per capita between $1,135 ND $4,465, focusing on how the yield of the three main crops goblaly that are also essential for those economies can get affected by changes in temperature. The countries under study will be India, Nicaragua and 

Agricultural data from those countries is going to be subject of study, focusing on how the yield of their main crop that they have in common can be affected by weather condition.

Low and middle income economies were classified by [The World Bank](https://datahelpdesk.worldbank.org/knowledgebase/articles/906519-world-bank-country-and-lending-groups)

With machine learning it is possible to predict how crop yields can be affected by changes in precipitation, temperature and use of pesticides.

### Data Science Solution
This project aims to generate insights into how the yield production of specific crops can be affected by precipitation, temperature, and pesticides in 15 years. The crops' yield to be analyzed are going to be the top three with highest yield in Global South Countries. From that selection, the top four countries with highest yield are going to be our location for this analysis.

For this prediction five additional datasets are going to be joined to the dataset containing the target. Those are agri_land, cropland, country_are and dif_temp, pesticides. All of them are for public access on [FAO](https://www.fao.org/faostat/en/#data/QCL) and [World Data Bank](https://data.worldbank.org/indicator). 

### Impact Solution
Big variations in the food disponibility directly affect citizens, governments, national economies and international markets. So it is expected from this project:

. Predict how the yield rice in India is going to be affected by weather changes in the future

### Dataset Description

yield_df:  pesticides and yield
country_sup: provides information on the total area per country
agri_land: total agricultural land in the country
cropland:  total cultivated area per crop. 
pesticides: herbicides, insecticides, fungicides and bactericides, fungicides for seeds, insecticides for seeds and rodenticides used per crop in each country.
temp_soil: variation of temperature in the soil
All these datasets were collected from [FAOSTAT](https://www.fao.org/faostat/en/#data/QCL)

### Data Dictionary
country: The name of the country where the crop data was collected.<br>
crop: The type of crop for which the data is recorded.<br>
year: The year in which the crop data was collected.<br>
yield_ton_ha: The yield of the crop in tons per hectare.<br>
rain_mm: The amount of rainfall in millimeters during the crop-growing season.<br>
avg_temp: The average temperature in degrees Celsius during the crop-growing season.<br>
dif_temp: The difference in temperature (maximum - minimum) during the crop-growing season.<br>
country_sup: The supply of agricultural inputs in the country.<br>
agri_area: The agricultural area available for cultivation in hectares.<br>
crop_area: The area of land specifically used for growing the crop in hectares.<br>
fung_bac_ton_ha: The amount of fungicides and bactericides used per hectare.<br>
herb_ton_ha: The amount of herbicides used per hectare.<br>
insec_ton_ha: The amount of insecticides used per hectare.<br>
rodenticides_ton_ha: The amount of rodenticides used per hectare.<br>
fung_seed_ton_ha: The amount of fungicide-treated seeds used per hectare.<br>
insec_seed_ton_ha: The amount of insecticide-treated seeds used per hectare.

### Next Steps in the study
- EDA: null, duplicated, graphs
- split and scalled data
- evaluate models: logistic regression, random forest, knn
- compare models: metrics, accuracy, cross validation, learning curve. Check paper comparing the two df.
