## Analyzing-Road-Accidents-Using-Data-Mining-and-Machine-Learning-Techniques


### Motivation
- UK police forces collect data on every vehicle collision in the UK on a form called Stats19. [Kaggle Dataset Link](https://www.kaggle.com/silicon99/dft-accident-data)
- The dataset used in this project provides detailed road safety data about the circumstances of personal injury road accidents in GB from 1979, the types (including Make and Model) of vehicles involved and the consequential casualties.
- Such a dataset can be used to obtain behavioural patterns based on certain rules. From these rules, some conclusions can be extracted which can help to develop suitable prevention policies to reduce number of casualties in cases of such accidents.


### Objective
- The goal of this work is to analyze the main factors that could be the possible causes of road accidents in UK as per the dataset provided.

### Dataset
- Download the dataset from this [Google Drive link](https://drive.google.com/file/d/1TSbV13ftvywhoH7H9GfzDqIsAL-jQDsE/view?usp=sharing), unzip and cut-paste the three csv files to input folder

### Proposed work
- A selection of accident data is made, taking into account its relevance in our study, in order to work with a reasonable data source. The variable Number_Of_Casualties, chosen a priori, serves as output attribute.
- To remove the curse of dimensionality, feature selection tools and techniques were applied in a unique way to find best 18 predictor variables for the output variable Number_Of_Casualties.
- Various data mining models (like k-nn classifier, naive bayes classifier, decision tree etc) trained and tested on the dataset.
- A ranking of the most important predictors for the output variable Number_Of_Casualties is established based on these models.
- Association rules from decision trees for the predictor variables are obtained. These association rules allow the most relevant factors to be extracted to enable the output variable to be evaluated.


#### Step 1 : Selection & Pre-processing of accident data 
- There are 3 CSVs in the dataset useds. Accidents is the primary one and has references by Accident_Index to the casualties and vehicles tables. 
- After merging the three tables the given dataset had 961906 samples with around 67 variables in each sample.
- To start with pre-processing, the attributes having a lot of null entries were removed.  Dataset now had only 62 variables.
- Out of these 62, the variable Number_Of_Casualties measured the gravity of the accidents and hence it was chosen as the response or output variable.
