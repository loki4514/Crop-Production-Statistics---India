# Crop Production Statistics India

### Problem Description :
- The collection includes thorough statistics on India's crop production, broken down by state and district. The dataset spans the years 1997 to 2023 and includes data for the four principal crop seasons of kharif, rabbi, summer, and fall. The report offers details on the annual yield and production of crops farmed around the nation.
- Experts and farmers who are interested in understanding agricultural production patterns in various regions of India will find the dataset to be helpful. You can decide how to increase agricultural productivity in the nation by examining the data and figuring out the variables that affect crop yields and production.
- Since it is raw data, researchers can only study it however, it is possible to utilise the dataset to train machine learning models that can forecast crop yields and production in various regions of the nation.
- This information can be useful for agricultural enterprises and organisations. The dataset offers a thorough overview of crop production statistics in India, which is crucial for comprehending the nation's agricultural environment and creating successful sustainable agriculture plans.

### Dataset : 👉 https://www.kaggle.com/datasets/nikhilmahajan29/crop-production-statistics-india

### Exploratory Data Analysis and Data Cleaning : 
- Data Cleaning :- Data looks to be fine, there is no cleaning required

- Exploratory Data Analysis :- Several significant conclusions drawn from the analysis 👇
  - In India, the most widely grown crops are rice, maize, moong (green gramme), urad, and sesame.
  - Five states Punjab, Maharashtra, Rajasthan, West Bengal, and Madhya Pradesh have vast agricultural land.
  - Kerala, Goa, Tamil Nadu, Andaman & Nicobar Island, and Karnataka are India's top five agricultural producing states.
  - No matter how much land is used for agriculture and how much is produced, the yield should still be higher in order to boost the Indian economy and the profit of the farmer
  - States with highest yields include Puducherry, West Bengal, Kerala, Goa and Andaman & Nicobar Island.
  - The choice of a certain crop to increase production depends on numerous factors, including weather, geography, and others.
  - All of these data have been processed using ML models so that farmers can choose a precision crop that is suited to their region and increases the productivity.

### Model Building :
- As there are more values in the category columns, label encoding may be a frequently employed technique since target directed encoding is used to establish some sort of relationship with the target variable.
- Because it requires awhile to individually do each categorical encoding, replace a missing value, and normalise with a standard scalar, scikit learn pipeline is employed.
- A separate pipeline is created for categorical and numerical data, and these pipelines are combined with ColumnTransformer before the ML model is put to the pipeline. The dataset is divided into train and test phases.
- Throughout the pipeline, ML models such as Decision Tree, Random Forest, Xgboost, Catboost, and GradientBoost are used. Of them, XGBoost Regressor performs well when learning from data.

### Model Performance : 
- Model train scores are 99.7, 99.9, 99.8, 96.4, and 94.5 for Random Forest, Decision Tree, Xgboost, Catboost, and GradientBoost, respectively. 97.9, 96.9, 98.6, 96.9, and 94.5 are test scores.
- Random Forest, Decision Tree, Xgboost, Catboost, and GradientBoost have mean absolute errors of 6.13, 7.53, 6.82, 16.4 and 17.9. respectively. Root Random Forest, Decision Tree, Xgboost, Catboost, and GradientBoost have respective of 134.7, 162.19, 109.13,250.32 and 250.32.
- Observation : Other regression measures performance are mean absolute error is 6.82 and root mean squared error is 109.13, which has good score comparison to all. XGBoost Regressor has train accuracy of 99.8 and test accuracy of 98.6.


<img src="https://user-images.githubusercontent.com/80893814/224046262-518ce82d-e2ec-4ac4-ae82-626d0d31affd.png" width="400" style="max-width:100%;">











