# Predicting Model for Real Estate Prices


## Introduction

The objective of this work is to develop a model for predict prices of real estate assets. This model will be focused on real estate transactions carried out in several cities and will take as variables for de model different features, such as rooms or surface. After obtaining the results, it can be seen that the predictions have acceptable error rates. Finally, it is established as a line of work the extension of the prediction to a data set that covers all the cities of the entire country and includes a greater number of variables, with the aim of generalizing and improving the results obtained. 

This project uses the Scikit-learn Python library to determine the price prediction, given a data set of real estate assets. The approach to the problem is made through the use of Random Forest algorithm, training the model with a data subset and evaluating the performance with the remaining data set.

The project is written using Python 3.8.0 and Scikit-learn 0.21.0 and licensed under Apache License 2.0. Full source code is [available on the following link](https://github.com/Dparedero/Masters_Dissertation). 

In addition, the dissertation is exposed in detail (in Spanish) [on the following document](https://github.com/DParedero/Masters_Dissertation/blob/master/DissertationSpanish.pdf). 

### Use Cases
The project looks to address the following two use cases:

1. Price Prediction: Given a set of features of a real estate assets, being able to establish a reference price for this assets that matches the market. 

2. Feature Engineering: Improve the accuracy of the model finding which data columns make the most useful features and studing wich is the relative importance of these features into the model.

## Setting up the Data

### Data source

Properati SA is an Argentine real estate web portal, dedicated to the publication of assets for sale and rental transactions which operates in several Latin American countries, such as Argentina, Peru and Colombia. Since it opened in 2012, it has positioned itself as a leading portal in the Latin American sector and it is a reference thanks to the periodic publication that makes its own data for free use. This data sets are [available on the following link](https://www.properati.com.ar/data/) and it can be dowloaded in CSV or using the Google BigQuery interface.

Firstly, this are the filters that are applied to the BigQuery extraction:

· type: Propiedad. (property)

· country: Argentina. 

· created_on: greater than 01/06/2018 

· operation: Venta. (sale)

· currency: USD.

In addition, it is necessary to include the following filters to make sure that the dataset does not contain outliers:

· cities: Vicente López and Palermo.

· surface: less than 1000 m2.

· rooms: less than 10 rooms.

· bathrooms: less than 9 bathrooms.



Finally, [this is the dataset obtained](https://github.com/DParedero/Masters_Dissertation/blob/master/data/Dataset.csv), in CSV format.


## Predicting Model

### Performance metrics

### Random Forest algorithm

## Feature engineering
