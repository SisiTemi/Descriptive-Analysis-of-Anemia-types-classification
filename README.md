# Descriptive-Analysis-of-Anemia-types-classification
This project involves the development of a Machine Learning model that classifies various types of anemia. The classification is based on a descriptive analysis of data derived from complete blood count (CBC) tests specific to each anemia type.


i am happy to share my project with you,
I worked with a dataset i found on Kaggle called Anemia type classification
Which consists of 14 blood parameters 

The first thing i did was load the data into my python using jupyter notebook,
and this consists of 14 blood parameters.
FROM WBC TO PCT, 
AS you can see i also have my variable DIAGNOSIS.(which are Anemia types)

The aim of this project is to be able to classify Anemia type based on the blood parameters.

IN ORDER to achieve this,
The first thing i did was to make sure my data is clean,

IN checking the data structure, i found out that my data as 1281 entries and a total of 15 columns in the data.

i saw that they were in the right format and the i could see that all the blood parameters are float or numeric and the Diagnosis is an object as it should be.

Next thing i did was to check for missing values to know if my data is missing or not.
using the command .NULL and i discovered all the data are complete, which made me proceed to EXPLORATORY DATA ANALYSIS

First thing i did was describe my blood types which you can see that the AVERAGE WBC IS 7.87 AND THE others INDICATED IN THE RESULT BELOW.

in order to further explore the blood parameters with respect to its relationship,
i made a box plot, in which it will be able to represent the distribution of each of the blood parameters by the anemia types.

FIRST VISUALIZATION HERE IS THE WBC by the anemia
from here we can see the distribution of each and we can see a lot of outliers which need to be treated, 
in order to do so, we have to make the data consistent with each other.
DOING THAT, i use a standard scaler to rescale the data

THE NEXT PLOT I HAVE HERE IS 
The distribution of the anemia type, inside our data, we can see most of the people there are healthy, while only a very few has leukemia with

also in order to explore the relationship between each of this blood pressure, I used a HEAT MAP to visualize the correlation btw each of the blood parameters, 
from here we can see that a strong relationship or positive relationship btw HCT AND MCH, 
also HGB AND RBC

FOR all other Variable, there are weak or no relationship between them

HERE is where I standardize our data to make it consistent among the variables and also
I performed a DYMENSIONAL REDUCTION in order to reduce the number of variable that will fit the data.

ON TESTING THIS i wanted to make sure the variables contain at least 85% the variation of the original data,
doing so i found out 10 features were able to account for 85% of the variations in the data.

TO START THE Modelling, MY data was split into 30% test and 70% train set
and i fit in a support vector model, A KNN model AND RANDOM Forest MODEL

so on fitting the model on the original data, 
i achieved 0.90% accurarcy from the SVM

also 0.67% accuracy from the KNN

AND also 99% accuracy from the Random forest

so,we can also see the recall, precision & F1 SCORE for the Random forest here

in this i was able to conclude that Random Forest Model was able to perform better on the Original dataset
this model can predict 99% correctly in the the anemia

with this i have been able to develope a model to classify ANEMIA TYPE Based on the blood parameters with a good accuracy score
CONCLUSION (FOR PREDICTION)

when using THE ORIGINAL DATA WITHOUT SCALLING IT
(THIS PERFORMED BETTER THAN THE SCALED DATA)

MODEL 2 IS ONE 
I SCALED AND PERFORM PRINCIPAL ANALYSIS  AND REDUCED THE DIMENSION TO 10.
(THIS DIDNT PERFORM AS GOOD AS THE MODEL 1)


diff was deciding which model to display or use
