[Home Page](../index.md)

# Project Overview
## Problem Definition
- Accurately forecasting the stock market has always been a cornerstone of business research and development.
- Popular trading algorithms rely too much on technical analysis of basic indicators (High, Low, Open, Close, Volume)
- Research into inclusion of sentiment analysis only leverages official news outlets, which involve many biases.
- State-of-the-art deep learning models have seen very little application in this field. And the models initially explored have seen many incremental improvements since.

## Our Approach
- wGAN-GP is used over traditional GAN networks, for promotion of training stability and convergence. Improved forms of GAN networks have seen little implementation in the field of finance.
- The usage of sentiment analysis of data coming directly from the public, rather than from biased news outlets or similar feeds.
- Research into inclusion of sentiment analysis only leverages official news outlets, which involve many biases.
- State-of-the-art deep learning models have seen very little application in this field. And the models initially explored have seen many incremental improvements since.

# Full Project Pipeline
![Project Pipeline](ML%20Capstone%20Project%20Pipeline%20Diagram.png)

# How to run the wGAN-GP Stock Prediction Model

## Required Files

All the listed files must exist within the same directory on your machine.
- wGAN-GP model notebook* (located in their respective directories)
- ARIMA Model Notebook
- AE (autoencoder) Notebook
- `fulldata.csv` (located in the data directory)

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


*This project was inspired by [Using the latest advancements in deep learning to predict stock price movements](https://towardsdatascience.com/aifortrading-2edd6fac689d#5ec4)*
