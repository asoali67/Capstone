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
   a. looking for null data's
   b. Visualizing the target variable distribution and check the classification balance
   c. Visualizing the distribution of features "BMI" and "Weight" to target features "ObesityCatagory"
2. Break the data into test and train sets and do a pairplot to visualize the distribution of each feature with respect to the target class
3. Encode using OrdinalEncoder to encode the only string feature "Gender"
4. Now its time to create Models to analyse the data, as a prilimenary investigation i have used two main methods
   a. Using RandomForestClassifier
     i. to identify the optimal number of forests and use it.
    ii. Using RandomForestClassifier to identify the feature score to select only the features that is relevant to the classification
   iii. 

#### Results
What did your research find?

#### Next steps
What suggestions do you have for next steps?

#### Outline of project

- [Link to notebook 1]()
- [Link to notebook 2]()
- [Link to notebook 3]()


##### Contact and Further Information
