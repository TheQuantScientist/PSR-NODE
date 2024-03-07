# Introduction 

This project introduces an innovative method that combines Neural Ordinary Differential Equations (NODE) with Phase Space Reconstruction (PSR) to redefine accuracy and reliability in financial market predictions. By bridging the gap between the mathematical elegance of differential equations and the dynamic learning prowess of neural networks, our approach transcends the limitations of conventional forecasting techniques.

## Project Overview

Our research showcases the NODE model's exceptional performance across various stock categories, including technology, finance, and pharmaceuticals, where it surpasses traditional machine learning and deep learning benchmarks such as LSTM, RNN, CNN, and Transformer models. The findings reveal a remarkable up to 83% reduction in Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE) within the technology sector, with an average error reduction of about 77% in finance and pharmaceuticals. These results highlight the model's ability to navigate the intricate, non-linear dynamics of the market, proving its unparalleled precision in long-term forecasting. This paper not only challenges existing financial forecasting paradigms but also paves the way for new applications of differential equation-based models in market analysis. The synergistic use of PSR and NODE provides a solid foundation for future endeavors in algorithmic trading, investment strategy formulation, and extensive financial examination. We invite researchers, practitioners, and enthusiasts from the realms of machine learning, finance, and data science to explore our findings. This project is not just a step forward in financial forecasting; it's a leap towards a more informed and precise understanding of market behaviors.

## Features

- **Integration of Neural Ordinary Differential Equations (NODE) with Phase Space Reconstruction (PSR)**: This innovative combination leverages the mathematical modeling capabilities of NODEs and the dimensional transformation of PSR to create a powerful forecasting model.
Integration of Neural Ordinary Differential Equations (NODE) with Phase Space Reconstruction (PSR):
This innovative combination leverages the mathematical modeling capabilities of NODEs and the dimensional transformation of PSR to create a powerful forecasting model.

- **Phase Space Reconstruction for Feature Engineering:** The technique of PSR is applied to reconstruct the phase space of the input features, enhancing the model's ability to capture the underlying dynamics of the stock prices.

- **Custom ODEFunc Neural Network:** A custom neural network architecture (ODEFunc) defined for the differential function in the NODE framework, showcasing the flexibility in designing complex models.

- **Use of Time Series Split for Model Validation:** The application of TimeSeriesSplit for model validation respects the temporal order of the data, which is crucial for time series forecasting.

- **Early Stopping Mechanism:** Implementation of an early stopping mechanism to prevent overfitting, improving the generalizability of the model.
**Model Training with Validation Data:** The model is not just trained on a fixed training set; it's also validated on multiple folds of data, ensuring its robustness and reliability across different time periods.

- **Efficient Data Preprocessing and Scaling:** The detailed preprocessing steps, including scaling of features and target variables, ensure that the model receives data in an optimal format for learning.

## Technologies Used

- **Pandas:** Used for data manipulation and analysis, particularly for loading the stock price data from a CSV file and preprocessing it for the model.

- **NumPy:** Utilized for numerical computing, especially in the phase space reconstruction function to manipulate arrays and perform calculations efficiently.

- **Scikit-learn (sklearn):** This library is employed for its preprocessing capabilities (e.g., MinMaxScaler for feature scaling) and for splitting the dataset into training and validation sets (TimeSeriesSplit), as well as for evaluating the model's performance using metrics like mean absolute error (MAE) and root mean squared error (RMSE).

- **PyTorch:** A deep learning framework that is used to define the neural network models, including the custom ODE function (ODEFunc) and the NeuralODE model itself. It provides the infrastructure for model training, including automatic differentiation to compute gradients and optimizers (e.g., Adam) for updating model parameters.

- **torchdiffeq:** A specific library for integrating ordinary differential equations (ODEs) within PyTorch, used here to solve the ODE as part of the NeuralODE model (odeint function).

- **Copy:** A standard Python library used here for deep copying model states, enabling the implementation of early stopping by keeping track of the best model weights during training.

## Getting Started

Follow the instructions in the subsequent sections to set up your environment, train the model with your dataset, and evaluate its performance on stock price forecasting tasks through evaluation metrics of MAE and RMSE. This model has been tested on various datasets of prominent technology, financial, and pharmaceutical companies, demonstrating its capability to accurately capture market trends, fluctuation groups, instant downtrends, surpassing RNNs-based models.

