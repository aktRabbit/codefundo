# Flood prediction Model
### Abstract

A flood prediction model can play a key role in providing relevant information of possible impending floods in populated locations. The development of such models can reduce the damage in areas by decreasing the economic and environmental impacts of floods. More importantly, a prediction system developed for India, especially the Kerala area, can effectively lower the risk of harm and loss of life. If artificial neural network (ANN) models can provide sufficiently accurate forecasts, even one day ahead, the lead time for flood warning can be extended and the subsequent flood emergency measures can be better planned and executed.

The risk of flood is affected by factors such as land use, meteorological events,hydrology and the topology of the land.In this  project,we can explore the use of artificial neural network models to predict the onset of floods. Rainfall is considered as the primary factor influencing the likelihood of flood .

The mean percentage accuracy and correlation coefficient can be used to evaluate the performance of trained neural networks. A feed-forward model with six input neuronal units, four hidden units and one output unit can be used to produce the best predictive results for this type of neural network .

##### Objectives :-
- The main objective of this study is to research and develop artificial neural networks that can be used as model to predict the onset of floods.
- To pre-process historical weather data into a form that is suitable for training neural networks and to identify the salient variables for training neural networks.

### Data Preparation
we can access a wide verity of meteorological data from the links listed in https://sites.google.com/site/geometocea/home/online-links/online-data-links as well as many more sources.we can use reanalysis data available from NOAA (NCEP/NCAR) or ECMWF (ERA).We can also consult India Meteorological Department (IMD) to get some station data.

### Data set generation
- Split-sample training is a common ANN training method .The basic idea behind this approach is to withhold a small subset of the data for validation, and to train the network on the remaining data.
- The cross validation technique can also be used in ANN training.
### Data pre-processing
The data can be divided into sub-sets for training, validation
and testing. The output of a neural network is typically between 0 and 1 therefore the raw rainfall figures have to be scaled to a range between 0 and 1 before it can be used as input. Feed-forward neural network architecture can be considered in all of the initial datapre-processing.
### Model design
#### Data normalization :
As we mentioned above, the split-sample training is a common method to train ANN models. The 15-20 years data obtained can be divided into training,validation and test data sets after it had first been normalized to a certain range.The observed historical data for rainfall will be first normalized within a range of 0.1...0.9 as the ANN model can be the sigmoid transfer function.The normalized data will then be presented to the ANN model at the input layer.
#### Model parameters :
The historical rainfall data in millimetres, will be used in this study since the advantage of our approach is that it
does not require many variables and very little knowledge of the flooding domain.The model parameters such as the number of epochs were varied to achieve improved performance by conducting several training.
### Real valued outputs
The raw data can be scaled by calculating the maximum (Rmax ) value and minimum (Rmin ) value over a n entire data set and for each rainfall value (ri ) in the set. Equation below shows the transformation used for scaling, where Rmax and xmin are the maximum and minimum rainfall values, ri is the original, and xi is the scaled value.

##### Equation :-
- xi = (ri - Rmin) / (Rmax - Rmin)
 
