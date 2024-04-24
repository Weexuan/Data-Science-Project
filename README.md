# SC1015 Mini Project - Heart Disease Analysis & Prediction

Heart disease is a leading cause of mortality worldwide, our group will be exploring the causes of heart disease and create predictive models to support timely interventions and reduce the associated health burden.
![](https://github.com/Weexuan/Data-Science-Project/blob/main/others/Cover%20Image.png)
## Contribution

Koh Wee Xuan - Exploratory Analysis, Convolutional Neural Network, Decision Tree, Exploring Further Machine Learning Techniques

Woo Weng Tai - Data Processing, Exploratory Analysis, Logistic Regression, Exploring Further Machine Learning Techniques

Teo Liang Wei, Ryan - Data Processing, Exploratory Analysis, Logistic Regression, Random Forest

## Exploratory Analysis

For our exploratory analysis, we analyze how some of the variables in the dataset affect an individual’s risk of attaining heart disease in ten years.

The risk of being affected with heart disease in ten years increases by 66.96% if you are a male, and as you get older with an increase of 7.66%  per year.

If one is a smoker, there will be an 18.3% higher chance of being affected, and every cigarette smoked per day further increases it by 1.64%.

For those diabetics, they are 150.87% more likely to be affected and per unit increase in BMI further ups the odds by 4.96%.

Those with high cholesterol levels are 49.77% more likely to be affected and those with high blood pressure are 95.68% more likely to.

## Machine Learning Techniques
After doing exploratory analysis, we attempted different machine learning techniques to predict the risk of heart disease using all the variables as the predictor, and the TenYearCHD as the response variable.
### Logistic Regression

The first method we use is logistic regression. We decided on this model as is used for binary classification tasks where there are only 2 possible outcomes, true or false and it assumes a linear relationship between the variables and the log odds of the outcome seen from the correlation coefficient graph earlier. Using this, we have obtained an accuracy of 88.39% with a true positive rate of 2.35% and a true negative rate of 99.8%.

### Decision Tree
The next model we will be covering is the decision tree. The Decision Tree is capable of handling our mixed data types conveniently. It provides insight into the importance of specific factors for making predictions by examining the splits in the trees. Using this we have obtained an accuracy of 78% along with a true positive rate of 30.5% and a true negative rate of 84.3%.

### Random Forest
Random forest is similar to a decision tree but instead, it merges multiple of it. When dealing with classification, each tree predicts a class label of a new data point, and its final prediction result is based on the class with the most ‘votes’. For regression, the average prediction made by all the trees will be used for the final prediction. Using this we have obtained an accuracy of 88% along with a true positive rate of 1% and a true negative rate of 99.8%.

### Convolutional Neural Network
Throughout the learning process, we realized that the dataset that we had chosen was lacking. Even though we were able to create a model that predicts whether a patient is at risk of heart disease, we recognize that the results we obtained were not favorable due to the low true positive rate. 

Therefore, to further aid in our learning, we will be attempting to do a simple convolutional neural network model using a different dataset. This new dataset is composed of CT scan images that we can use to predict the risk of heart disease.

The idea is that if we could potentially obtain a dataset that has a patient’s demographic tied to his CT scan image, we would be able to create a more effective prediction model.

We were able to utilize TensorFlow to create a simple self-trained model with a validation accuracy of 73.81%. It is capable of predicting the chances that a patient is suffering from cardiomegaly.

## Conclusion
This assignment was a good project that allowed us to better understand the implications of neglecting our health. We were also able to create a model that gives a prediction on whether we are at risk of coronary heart disease, albeit at a lower accuracy. 

In the future, we believe that if we can obtain a dataset that has a patient’s CT scan tied to his demographic, we will be able to create a better model that can accurately predict a patient’s risk of having heart disease.

## References
https://www.kaggle.com/datasets/aasheesh200/framingham-heart-study-dataset

https://www.kaggle.com/datasets/rahimanshu/cardiomegaly-disease-prediction-using-cnn

https://tahera-firdose.medium.com/filling-missing-values-with-mean-and-median-76635d55c1bc#:~:text=When%20to%20fill%20missing%20values%20with%20the%20median%3A,less%20influenced%20by%20extreme%20observations.

https://www.datacamp.com/tutorial/understanding-logistic-regression-python

https://towardsdatascience.com/random-forest-in-python-24d0893d51c0

https://www.kaggle.com/code/mmdatainfo/k-nearest-neighbors
