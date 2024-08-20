# Challenge Module 19
## Neural Network Challenge 2: An ASU AIML Challenge by CA Frisby

### Overview
Import a .csv file from an online source.  Prepare the data for
a neural network model.  Compile and evaluate the model using a deep neural
network.  Predict the attrition and attrition by department.  Discuss 
further recommendations regarding attrition predictions.  
This is strictly an academic model. 

References:  Starter code was provided by ASU AIML. 
             
### Part 1:  Prepare the data.

The data set including multiple formats and more columns that required.  Ten
columns were selected for input or "X". 
The output are two separate 'y' variables, Attrition and Department.
StandardScaler was used to scale the float point numbers in the "X" data set.  
Onehotencoder was used for categorical X and y data. 

### Part 2:  Create, compile and train a neural network model.
A deep neural network was created with two branched output layers and two
shared layers.  
A  model was set up with the following parameters:
    1.  One hidden layer and one output layer wer designated for a branch to 
        predict Department.
    2.  One hidden layer and one output layer wer designated for a branch to 
        predict Attrition.
The model was compiled and fit using the binary crossentropy loss function, the
adam optimizer, and the accuracy evaluation metric.  Execution was set to 10
epochs. 

### Part 3: Predict attrition and department.
Department Predictions Accuracy: 0.95923912525177
Attrition Predictions Accuracy: 0.8288043737411499



