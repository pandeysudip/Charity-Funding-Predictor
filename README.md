# charity-funding-predictor

## Background

Used machine learning and neural networks to create a binary classifier that is capable of predicting whether applicants will be successful if funded.

Datasets containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

* **EIN** and **NAME**—Identification columns
* **APPLICATION_TYPE**—Alphabet Soup application type
* **AFFILIATION**—Affiliated sector of industry
* **CLASSIFICATION**—Government organization classification
* **USE_CASE**—Use case for funding
* **ORGANIZATION**—Organization type
* **STATUS**—Active status
* **INCOME_AMT**—Income classification
* **SPECIAL_CONSIDERATIONS**—Special consideration for application
* **ASK_AMT**—Funding amount requested
* **IS_SUCCESSFUL**—Was the money used effectively



###  Preprocess the data

Using your knowledge of Pandas and the Scikit-Learn’s `StandardScaler()`, you’ll need to preprocess the dataset in order to compile, train, and evaluate the neural network model later in Step 2

Using the information we have provided in the starter code, follow the instructions to complete the preprocessing steps.

1. Read data to a Pandas DataFrame and made IS_SUCCESSFUL column as target.
2. Droped the `EIN` and `NAME` columns.
3. Determined the number of unique values for each column.
4. For those columns that have more than 10 unique values, determine the number of data points for each unique value.
6. Used the number of data points for each unique value to pick a cutoff point to bin "rare" categorical variables together in a new value, `Other`, and then checked if the binning was successful.
7. Useed `pd.get_dummies()` to encode categorical variables

###  Compiled, Trained, and Evaluate the Model

Designed a neural network, or deep learning model, to create a binary classification model that can predict if an Alphabet Soup–funded organization will be successful based on the features in the dataset. 
1. Created a neural network model by assigning the number of input features and nodes for each layer using Tensorflow Keras.
2. Created the first hidden layer with 15 nodes and relu activation function.
4. Added a second hidden layer with 8 nodes and relu activation function.
5. Created an output layer with an sigmoid activation function.
6. Checked the structure of the model.
7. Compileed and trained the model.
8. Created a callback that saves the model's weights every 5 epochs.
9. Evaluated the model using the test data to determine the loss and accuracy.
10. Saved the model to HDF5 file, and name it `AlphabetSoupCharity.h5`.

### Optimized the Model

Optimized the model using kerastuner. 
* Adding more neurons to a hidden layer.
* Adding more hidden layers.
* Using different activation functions for the hidden layers.
* Adding or reducing the number of epochs to the training regimen.


## Summary



