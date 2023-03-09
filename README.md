# BILSTM−BIGRU: A FUSION DEEP NEURAL NETWORK FOR PREDICTING AIR POLLUTANT
With the spirit of reproducible research, this repository contains all the codes required to produce the results in the manuscript:

>Prasanjit Dey, Soumyabrata Dev, Bianca Schoen Phelan, "BILSTM−BIGRU: A FUSION DEEP NEURAL NETWORK FOR PREDICTING AIR POLLUTANT" under review in IGARSS2023

### Executive Summary:
Predicting air pollutant concentrations is an efficient way to prevent incidents by providing early warnings of harmful air pollutants. Accurate prediction of air pollutants is an important factor in controlling and preventing air pollutants. This paper proposed a bidirectional long-short-term memory and a bidirectional gated recurrent unit (BiLSTM−BiGRU) to predict PM2.5 concentration in the target city for different lead times. BiLSTM extracts preliminary features, and BiGRU further extracts deep features of air pollutant and meteorological data. The fully connected (FC) layer receives the output and make the accurate prediction of the PM2.5 concentration. The model is then compared with five other deep learning models in terms of root mean square error (RMSE), root mean absolute error (RMAE) and correlation (R2) over different lead times. The results indicate that the proposed model has at least 2.2 times lower RMSE than other models.

### Data:
The experiment used past pollution levels and meteorological parameters from Wanshouxigong, China, between March 1, 2013, and February 28, 2017 (each hour interval total 35060 hours). The dataset contains 12 pollutant and meteorological variables, such as PM2.5, PM10, SO2, NO2, CO, O3, temperature, air pressure, humidity, rain, wind direction, and wind speed.

### Code:
All codes are written in `python3`.

### Proposed Framework:
![Architecture](https://user-images.githubusercontent.com/49582829/206673155-9506eb1e-c59b-4df6-b25a-30d16d28e56b.png)
Fig. 1. Frameworks of the Fusion-based deep neural network for PM2.5 concentration prediction. x(t−i) is the pollutants con-
centration and meteorological data input in the model for each timestamp.

### Result:
![Result](https://user-images.githubusercontent.com/49582829/206673614-448dcb86-63c2-43db-a8d1-31464b0bc062.png)
Fig. 2. Fitting trend of the different model for the 0 to 180 lead-times. (a)−(f) represent the fitting trends of BiLSTM−BiGRU,
CNN−LSTM, CNN−GRU, CNN, LSTM and GRU models.

