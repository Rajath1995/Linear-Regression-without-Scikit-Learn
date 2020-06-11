# Linear-Regression-without-Scikit-Learn
This project creates a Linear regression model function which does not uses Scikit Learn.

Develop My Regression Function which handles multiple output datasets, implements simple linear
and Polynomial regression. Scalling and Regularization of the dataset is implemented. The function
written is then applied to manually generated one-Dimension equation for various noise level.
Finally the performance of the function is evaluated on the UCI datasets - AIRFOIL, SLUMP AND
YACHT HYDRODYNAMICS data set. Mean squared error for each of the scenario is recorded
and Graphs have been plotted when neccessary.

1.1 My Regression Function ALgorithm
1.1.1 Step1: Scaling and Regularization:-
Using Normalization for Scaling - Subtracting by mean of each column and dividing by standard
deviation(Standardization). Using Gaussian regularization technique. Gaussian Regularization
- exp(x − ￿ j )2/2s2
1
1.1.2 Step2: Spliiting the data input and target variables:-
Splitting the training data input and ouput variables into 5 equal sets for cross validation. Get
the splits for Polynomial and Simple Linear regression models in this step.
1.1.3 Step3:- Calculating the coeffecients using the cross validation:-
In cross validation one split will be validation set and rest splits will be used to calculate the set
of coeffecients/weights for Simple and Polynomial linear regression. Using the formula given
below:-
Φ † ￿ ((Φ T. Φ)^− 1 ).(Φ T ).(t k)
Repeat this process for 5 times i.e. to obtain a 5 fold cross validation.
1.1.4 Step4:- Selection of the best model:-
Getting the best coefficient set for both Simple and Polynomial models by comparing the
mean square error. Apply the model to whole training data we compare the mean square error.
Select the model with least mean square error.
1.1.5 Step5:- Apply the selected model to Test Dataset:-
After comparison of the Mean square errors obtained, the coeffecients obtained is applied to the
entire test set and predtictions are obtained.
MSE = frac{1}{N}sum_{i=1}^{N}(Y_i -{Y}_i hat)^2

Conclusion :

A simple linear, polynomial Regression function has been developed and cross validation has been
implemented. Various steps taken to improve the model selection through the implementation of
Gaussian Basis function. Generation of manual data from the given equation, the results obtained
were fairly good with little higher Mean Squared Error values.
