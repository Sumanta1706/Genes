# Genes
The steps involved in building a machine learning model is:
Reading the data, preprocessing the data, splitting into train-test , build models, selecting a model and evaluating the performance
### Preprocessing used 
For the preprocessing part, first of all we had to split our ‘Genotype’ column into 14 different new columns. Every new column is consisting of each character from the ‘Genotype’ column. 
Since our dataset contains many categorical values, in-order to use those categorical value for programming efficiently we created dummy variables. After creating dummies for all of our dependent variables we split our dataset into training (80%) and testing (20%) data.
### Input features
After creating the dummy the input features for each column are in 0 or 1 format. In each column 1 represents the corresponding category like; ‘A’, ‘C’ etc, and other features are formed 0. 
### Selected Model & Architecture and why
For our model we have used two different approaches to predict our model. The first model we have selected was random forest regression, and for our second model we have selected a neural network model, Keras sequential regression. 
For our Random Forest regression model, we have taken 3 different estimators, 100, 200 & 300. The maximum depths we have taken are 10, 50, 100 and maximum features are: 6, 8, 10, 12, 14, and 16. We have done a hyper parameter tuning for our train and test models using cross validations, and tried to fit our model accordingly. We managed to find the r2 value and both mean square and average errors. 
Now, for our neural network model, we have taken Keras sequential regression as our regressor. First we define our model by adding some dense layers in our model (as 9, 4 and finally 1). We used the activation method ‘relu’ for first two layers and then ‘linear’ for our final layer. Then we train our model using the defined model with 200 epochs.   
