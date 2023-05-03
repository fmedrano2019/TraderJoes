# How to run the wGAN-GP Stock Prediction Model

Detailed below is a stepped instructional to generate predictions with the wGAN-GP prediction model.


## Required Files

All the listed files must exist within the same directory on your machine.
- wGAN-GP model notebook* (located in their respective directories)
- ARIMA Model Notebook
- AE (autoencoder) Notebook
- fulldata.csv (located in the data directory)

**Directions which follow are equivalent for all forms of the wGAN-GP model (3-day, 5-day, etc).**

## Kernel Set Up
The following packages must be installed in the kernel you wish to run the notebooks with. These notebooks use Python 3.9.13.
- Pandas (1.4.4)
- Tensorflow (2.11.0)
- Numpy (1.21.5)
- Matplotlib (3.5.2)
- Scikit-learn (1.0.2)
- Statsmodels (0.13.2)
- Pytorch (2.0.0)
- torchviz* (0.0.2)
- torchsummary (1.4.5)

\*To use torchviz for architecture visualizations, [Graphviz](https://graphviz.org/download/) must be installed.

## Running the Notebooks

Once the kernel is set up, you can follow the directions below to generate stock closing price predictions.

1. Run the ARIMA notebook to generate ARIMA predictions for the dataset.
2. Run the AE (autoencoder) notebook to produced the autoencoded feature set.
3. Run the respective wGAN-GP notebook for final predictions.

## Full Project Pipeline
![Project Pipeline](ML&#32;Capstone&#32;Project&#32;Pipeline&#32;Diagram.png)

## Best Predictions
![Closing Price Predictions](3-day/visuals_withSentiment/3day_valandtestpreds.png)  
These results were gained from the 3-day wGAN-GP model.  
  
**Evaluation Metrics:**  
RMSE: 4.401446815516941  
NRMSE: 0.08795856784549294  
MAE: 3.4469847679138184  
MAPE: 0.022908411920070648  

## wGAN-GP Generator and Discriminator Execution Traces
### Generator
![Generator Execution Trace](3-day/visuals_withSentiment/3day_generatorArch-1.png)
### Discriminator
![Discriminator Execution Trace](3-day/visuals_withSentiment/3day_discriminatorArch-1.png)

*This project was inspired by [Using the latest advancements in deep learning to predict stock price movements](https://towardsdatascience.com/aifortrading-2edd6fac689d#5ec4)*

