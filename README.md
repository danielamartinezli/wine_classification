# wine
Evaluating different model prediction to classify wine

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
It would be beneficial for the wine industry because knowing before hand the class of wine they are generating could help to stimate profitability and better information about the type of wine cusomers are purchasing.

### Dataset Description
[Datasets:](https://archive.ics.uci.edu/dataset/109/wine)<br>
features:  contains information regarding chemical quality of three classes of wine.<br>
target: dataset containing the three classes of wine.<br>
wine: final dataset generate to create some visualizations.

### Data Dictionary
Alcohol: The alcohol content in the wine, typically measured in percentage by volume.<br>
Malicacid: The concentration of malic acid in the wine, which contributes to its tartness.<br>
Ash: The amount of ash present in the wine, which may indicate mineral content.<br>
Alcalinity_of_ash: The measure of the alkalinity of the ash in the wine, which can affect its taste and stability.<br>
Magnesium: The concentration of magnesium in the wine, which can influence various aspects of wine quality including taste and color.<br>
Total_phenols: The total amount of phenolic compounds present in the wine, which contribute to its color, flavor, and antioxidant properties.<br>
Flavanoids: The concentration of flavonoids in the wine, which are a type of phenolic compound known for their antioxidant properties and contribution to wine flavor.<br>
Nonflavanoid_phenols: The concentration of phenolic compounds in the wine that are not flavonoids.<br>
Proanthocyanins: The concentration of proanthocyanins in the wine, which are a subgroup of flavonoids contributing to color, taste, and antioxidant activity.<br>
Color_intensity: The intensity of color in the wine, which can be influenced by various compounds including phenolic compounds.<br>
Hue: The hue or shade of the wine color, often measured in degrees.<br>
0D280_0D315_of_diluted_wines: The absorbance at 280/315 nm of diluted wines, which can provide information about the concentration of various compounds such as anthocyanins and phenolic compounds.<br>
Proline: The concentration of proline, an amino acid, in the wine, which can influence taste and aging potential.

### Next Steps in the study
- evaluate models:knn random forest, <br>
- HYPERPARAMTERS<br>
. for knn:gridsearch, tunel model<br>
. two for each model<br>

- METRICS:<br>
. score for accuracy<br>
. f1 score*<br>
. learning curve<br>

- Analysis<br>
. two papers
