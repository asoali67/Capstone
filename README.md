<h1>Classification of person's obesity </h1> 

**Author** Aso Ali

<h2>Executive summary</h2>

<h4>Project overview and goals</h4>
The objective of this exercise is the ability to predict person's body type and its obesity level based on certain criteria like Age, Gender, Height, weight, BMI and physical activity level. The prediction will classify the person to one of these categories; Normal Weight, Obese, Overweight, Underweight.


<h4>Rationale</h4>
Obesity severely strains the healthcare system, driving nearly $173 billion in direct annual medical costs in the U.S. alone. It dramatically increases the risk for chronic diseases—such as type 2 diabetes, heart disease, and some cancers—while challenging daily operations with higher surgical complication rates and specialized equipment needs.
Obesity significantly increases healthcare costs, driving up U.S. direct medical expenses by nearly $173 billion annually (according to the Centers for Disease Control and Prevention). Adults with obesity incur medical expenditures that are roughly double or 36% to 100% higher than those of normal-weight individuals, with costs escalating alongside the severity of the condition and related chronic illnesses.

<h4>Research Question</h4>
To classify a new sample of the population to Obesity level, and to understand is the population obesity level is increasing or decreasing overtime. This will help to predict weather the population health risks increased or decreased overtime and also gives an idea of how the health trend will be in the future.

<h2>Model Outcomes or Predictions</h2>
The problem is a classification problem and all the models used are supervised machine learning models. For this project i will be using five different models 
<ul>
  <li>RandomForestClassifier</li>
  <li>LogisticRegression</li>
  <li>KNeighborsClassifier</li>
  <li>DecisionTreeClassifier</li>
  <li>SVC (Support Vector Classifier)</li>
</ul>
The out put of these model will include the Accuracy, Precision, Recall adn f1 scores in the form of a table 
</br></br>
<img width="666" height="35" alt="output table header" src="https://github.com/asoali67/Capstone/blob/main/images/output%20table%20header.png" />



<h2>Data Set Information</h2>
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
