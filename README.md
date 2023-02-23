# Recession Forecasting with GAN-Generated Synthetic Time Series Data
This project generates synthetic Treasury Bond yield time-series data from a DoppelGANger model and tests its ability to predict recessions. The associated paper can be found here: https://arxiv.org/abs/2302.10490.

### Data Folder
* Contains raw data for synthetic data generation, as well as synthetic data used in paper.
## Notebooks
### DGAN_generation
* Trains DoppelGANger (DGAN) model to produce synthetic data for forecasting task, tests fidelity metrics, and generates plots.
### DGAN_generation_classifier
* Trains DoppelGANger (DGAN) model to produce synthetic data for recession prediction task, tests fidelity metrics, and generates plots.
### synthetic_forecasts
* Uses real, synthetic, and combined data to forecast 1-year and 10-year Treasury yields at 1-day and 15-day horizons. Utilizes simple AR and LSTM models.
### synthetic_recession_classifier
* Uses real, synthetic, and combined data to predict upcoming recessions using classification models that generate probability of recession estimates. Utilizes logistic regression and LSTM-based classifier.
