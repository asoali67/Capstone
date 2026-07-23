### Classification of person's obesity 

**Author** Aso Ali

#### Executive summary
The objective of this exercise is the ability to predict person's body type and its obesity level based on certain criteria like Age, Gender, Height, weight, BMI and physical activity level. The prediction will classify the person to one of these categories; Normal Weight, Obese, Overweight, Underweight

#### Rationale
Obesity severely strains the healthcare system, driving nearly $173 billion in direct annual medical costs in the U.S. alone. It dramatically increases the risk for chronic diseases—such as type 2 diabetes, heart disease, and some cancers—while challenging daily operations with higher surgical complication rates and specialized equipment needs.

#### Research Question
To classify a new sample of the population to Obesity level, and to understand is the population obesity level is increasing or decreasing overtime. This will help to predict weather the population health risks increased or decreased overtime and also gives an idea of how the health trend will be in the future.

#### Data Sources
I have obtained the date from [Kraggle](https://www.kaggle.com/datasets/mrsimple07/obesity-prediction) The data seem to be balanced and small in size for this exercise not missing data’s to clean..

#### Methodology
1. Investigating the data and identifying the features and the target
   * Looking for null data's
   * Visualizing the target variable distribution and check the classification balance
   * Visualizing the distribution of features "BMI" and "Weight" to target features "ObesityCatagory"
2. Break the data into test and train sets and do a pairplot to visualize the distribution of each feature with respect to the target class
3. Encode using OrdinalEncoder to encode the only string feature "Gender"
4. Now its time to create Models to analyses the data, as a preliminary investigation i have used two main methods
   * Using RandomForestClassifier
      * Identify the optimal number of forests and use it.
      * Identify the feature score to select only the features that is relevant to the classification
      * Run the model and obtain the Out Of Bag score and the classification report that has the metrics
      * The other models i used all of Knn, Logistic Regression, Decision tree and SVM to obtain the metrics accuracy, precision, recall and f1 score


#### Results
The scores obtained from Random Forest was very high oob 0.997, and the report gave a very high score for each class, for the rest of model the score were lower but also high like 0.8 and higher
this result does concern me to look for reasons behind such high score, such as looking at the bias and variance. 
Note i have not tuned these models to its optimal.

#### Next steps
improve the models by using GridSearchCV to fined the best hyper parameters and identify the reason behind the high score i have obtained and weather i have overfitting or underfitting.

#### Outline of project

- [kaggle](https://www.kaggle.com/datasets/mrsimple07/obesity-prediction)
- [Capstone jupyter notebook](https://github.com/asoali67/Capstone/blob/main/Capstone.ipynb)


##### Contact and Further Information
