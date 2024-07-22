# Wine Quality Classification
Evaluating different model predictions for wine quality classification.

### Overview 

The problem area focuses on addressing the challenges associated with wine quality prediction from a consumer market perspective. Consumers, including wine enthusiasts, casual drinkers, and industry professionals responsible for wine selections, often face uncertainty when choosing wines based on subjective quality assessments. The goal is to develop a robust predictive model that accurately assesses wine quality using objective criteria, empowering consumers to make informed purchasing decisions.

Addressing this concern in some consumer could benefit:
- Wine enthusiasts seeking guidance on new wine selections.
- Casual drinkers looking for accessible information to navigate wine choices confidently.
- Professionals curating wine lists for restaurants or events, aiming to align offerings with customer preferences.

### Data Science Solution
The proposed solution leverages machine learning techniques to predict wine quality classification based on key characteristics. This involves:
- Utilizing supervised learning algorithms to classify wines into quality categories (low and high) based on features like fixed_acidity, volatile_acidity, citric_acid, residual_sugar, chlorides, free_sulfur_dioxide, total_sulfur_dioxide, density, pH, sulphates and alcohol.
- Implementing logistic regression analysis to predict continuous quality scores, KNN, Random Forest and AdaBoost, providing nuanced assessments of wine characteristics.

### Impact Solution
The implementation of an accurate wine quality prediction model offers several impactful outcomes:
- Empowering consumers to make informed wine purchasing decisions aligned with their preferences and reliable guidance on wine selections.
- Promoting a culture of informed consumption and appreciation for wine, enhancing overall enjoyment and value for consumers and industry professionals.

### Dataset Description
[Datasets:](https://archive.ics.uci.edu/dataset/109/wine)<br>
features:  contains information regarding chemical quality of three classes of wine.<br>
target: dataset containing the three classes of wine.<br>
wine: final dataset generate to create some visualizations.

### Data Dictionary
- Alcohol: The alcohol content in the wine, typically measured in percentage by volume.<br>
- Malicacid: The concentration of malic acid in the wine, which contributes to its tartness.<br>
- Ash: The amount of ash present in the wine, which may indicate mineral content.<br>
- Alcalinity_of_ash: The measure of the alkalinity of the ash in the wine, which can affect its taste and stability.<br>
- Magnesium: The concentration of magnesium in the wine, which can influence various aspects of wine quality including taste and color.<br>
- Total_phenols: The total amount of phenolic compounds present in the wine, which contribute to its color, flavor, and antioxidant properties.<br>
- Flavanoids: The concentration of flavonoids in the wine, which are a type of phenolic compound known for their antioxidant properties and contribution to wine flavor.<br>
- Nonflavanoid_phenols: The concentration of phenolic compounds in the wine that are not flavonoids.<br>
- Proanthocyanins: The concentration of proanthocyanins in the wine, which are a subgroup of flavonoids contributing to color, taste, and antioxidant activity.<br>
- Color_intensity: The intensity of color in the wine, which can be influenced by various compounds including phenolic compounds.<br>
- Hue: The hue or shade of the wine color, often measured in degrees.<br>
0D280_0D315_of_diluted_wines: The absorbance at 280/315 nm of diluted wines, which can provide information about the concentration of various compounds such as anthocyanins and phenolic compounds.<br>
- Proline: The concentration of proline, an amino acid, in the wine, which can influence taste and aging potential.

### Data Collection and Methodology
One dataset was collected from UC Irvine. Exploratory analysis was performed, creating a binary column for classification.
The data was balanced using upsampling, downsampling, and SMOTE. KNN, Logistic Regression, Random Forest, and AdaBoost were evaluated to train this data in combination with different scalers (MinMax, Standard, and Robust). 
Metrics such as Accuracy Score, F1, Precision, Recall, and Learning Curve were estimated.

### Limitations
The level of data imbalance can potentially negatively affect the evaluation metrics used to assess a model's performance. Even when the data has been balanced using SMOTE (Synthetic Minority Over-sampling Technique), which adds variability with the additional synthetic data. Predicting Class 1 accurately remained the most challenging aspect for all the models, even for Random Forest with SMOTE.

### Future Research
a. Feature engineering:
- Select the most discriminative features for this classification task.

b. Balance Data
- Weight Class with class_weight parameter

c. Models
- XGBoost
- Neuronal Networks
- Balanced Random Forest


### Conclusion
The original data exhibits imbalance in its class distribution, leading to inaccurate precision in classifying each category (resulting in false positives). To address this, they were balanced using both upsampling downsampling, and SMOTE techniques. SMOTE had the best score with any model evaluated. 
The model that achieved the best accuracy score, recall, precision, and F1 Random Forest model implemented on balanced data with SMOTE performed the best in predicting classes. However, accurately predicting Class 1 remained the most challenging aspect for all the models, including Random Forest with SMOTE.



