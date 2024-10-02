README FILE:
This repository contains a project focused on forecasting significant waveheight using various deep learning models such as LSTM, RNN, GRU, and their ensembles (RNN-LSTM, GRU-LSTM , GRU-RNN and RNN-LSTM-GRU). The models are evaluated using two key metrics: Prediction Interval Coverage Probability (PICP) and Mean Prediction Interval Width (MPIW).
Table of Contents :
•	Introduction
•	Data Collection
•	Data Preprocessing
•	Model Building and Training
•	Model Evaluation
•	Results
Introduction
The goal of this project is to develop and evaluate deep learning models to forecast significant wave height (WVHT) using data collected from the National Data Buoy Center (NDBC). The models are designed to provide prediction intervals, offering a range of possible future values.
Data Collection
Data is collected from the NDBC site, specifically targeting the following buoys for the years 2021 and 2022: 41001h2021, 41001h2022, 41002h2021, 41002h2022, 41009h2021, 41009h2022, 41010h2021 and 41010h2022. The dataset includes various meteorological and oceanographic parameters.
Data Preprocessing
The collected data undergoes several preprocessing steps, such as cleaning by removing the header row and converting relevant columns to numeric data types. The dataset is then filtered to extract observations recorded at specific intervals, such as every 60 minutes (1 hour). The datetime column is moved to the first position, and rows with WVHT values of 99 are filtered out. Finally, the data is sorted by datetime.
Model Building and Training
Various models are built and trained using the preprocessed data. The models include: LSTM, RNN, GRU, RNN-LSTM, GRU-LSTM, GRU-RNN, RNN-LSTM-GRU. The training process involves defining a quantile loss function and using it to train the models.

Model Evaluation
The models are evaluated using the PICP and MPIW metrics.
Results
The results are plotted and evaluated for each model. The plots show the actual values along with the prediction intervals.

Similarly, the same process has been applied to the other datasets.
