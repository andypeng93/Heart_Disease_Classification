# Modeling Heart Diseases Classification

**Author**: Andy Peng

The contents of this repository detail an analysis of the module 3 project. This analysis is detailed in hopes of making the work accessible and replicable.


### Business problem:

The task is to investigate heart diseases for a hospital. For this project we will be looking at a data set of patients in a hospital some with heart diseases and some without heart diseases. The main goal of this project is to keep an eye out for certain features that will allow us to categorize this patient as having heart disease.


### Data
Data can include whether the patient have heart disease or not and features relating to the patient such as age, sex, chest pain, resting blood pressure, maximum heart rate, etc.


## Methods
- Descriptive Analysis
- Modeling
- Choices made
- Key relevant findings from exploritory data analysis

## Results


#### Visual 1
<img src=./Visualizations/Gender.PNG width="800">
> Gender VS Heart Disease

#### Visual 2
<img src=./Visualizations/ChestPain.PNG width="800">
> Chest Pain Types VS Heart Disease

#### Visual 3
<img src=./Visualizations/Thal.PNG width="780">
> Thalium Stress Result VS Heart Disease

#### Visual 4
<img src=./Visualizations/Age.PNG width="800">
> Age of Individuals VS Heart Disease

#### Visual 5
<img src=./Visualizations/AgeMax.PNG width="820">
> Age of Individuals VS Maximum Heart Rate

#### Models
<img src=./Visualizations/ROC1.PNG width="780">
> ROC Curve of the different Models

<img src=./Visualizations/ModelResults.PNG width="780">
> Model Results of Base Model and Model Tuning

* AUC - Random Forest with GridSearchCV

* Accuracy/ F1 Score/ Recall - XGBoost

* Precision - Decision Tree with GridSearchCV



## Recommendations:

To summarize everything above, we can see from above that to correctly classified a patient as having heart disease we need to consider the following features.

1) Gender of the individual - Males have a higher chance at having heart disease than females.

2) Asymptomatic Chest Pain - Individuals with this type of chest pain have a high chance of having heart disease

3) Reversable Defect - If the thalium stress result turns out to be reversable defect, the individual would have a high chance of having heart disease.

4) Age & Maximum Heart Rate - As you get older, your maximum heart rate goes down. We can see that individuals that have heart disease tend to be older and have a lower maximum heart rate.

Our modeling shows that a regular XGBoost is the best model for our problem. This is because we want a model that generates a high recall value in order to minimize the chances of false negatives. Being that heart disease is extremely serious, mistakenly classifying a patient as false negative can be very dangerous. 


## Limitations & Next Steps

There are many features that we haven't considered. For example whether the family has a genetic disorder, body fat percentage, and the individual's diet. The model can be further improved by gathering more data.


### For further information
Please review the narrative of our analysis in [our jupyter notebook](./Heart%20Disease.ipynb) or review our [presentation](./SampleProjectSlides.pdf)

For any additional questions, please contact andypeng93@gmail.com


##### Repository Structure:

Here is where you would describe the structure of your repoistory and its contents, for example:

```

├── README.md                       <- The top-level README for reviewers of this project.
├── Heart Disease.ipynb             <- narrative documentation of analysis in jupyter notebook
├── presentation.pdf                <- pdf version of project presentation
└── Visualizations
    └── images                          <- both sourced externally and generated from code

```
