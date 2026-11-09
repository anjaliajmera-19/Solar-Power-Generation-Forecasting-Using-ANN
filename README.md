# Solar-Power-Generation-Forecasting-Using-ANN

**Objective**

The objective of this project is to predict solar power generation using weather conditions and solar-related parameters. The project uses historical meteorological data and solar geometry features to develop an Artificial Neural Network (ANN) model for estimating generated solar power.

The model aims to understand the relationship between environmental conditions and solar power generation and evaluate prediction accuracy using regression metrics.

**About the Dataset**

The dataset (solarpowergeneration.csv) contains 4,213 observations and 20 input features, along with one target variable (generated_power_kw).

The dataset includes the following parameters:

Weather Parameters: Temperature, relative humidity, atmospheric pressure, precipitation, snowfall, and cloud coverage.

Solar Parameters: Shortwave radiation, angle of incidence, zenith, and azimuth.

Wind Parameters: Wind speed and wind direction at different atmospheric levels, along with wind gust measurements.

Target Variable: Generated solar power in kW.

**Method**

The project consists of the following main steps:

Data Loading and Exploration: Loading the solar power dataset using Pandas and examining its features and statistical properties.

Data Preparation: Separating input features and target variables and dividing the dataset into training (75%) and testing (25%) sets.

Feature Scaling: Applying StandardScaler to normalize input features and target values.

Model Building and Training: Developing an Artificial Neural Network using TensorFlow and Keras with two hidden Dense layers containing 32 and 64 neurons, respectively, and ReLU activation.

Model Training: Training the ANN using the Adam optimizer, Mean Squared Error (MSE) loss function, batch size of 32, and 150 epochs.

Model Evaluation: Evaluating predictions using Root Mean Squared Error (RMSE) and R² score, along with actual-versus-predicted scatter plots.

**Requirements**

To run the project, install the following libraries:

NumPy

Pandas

Matplotlib

Seaborn

TensorFlow / Keras

Scikit-learn

Install using:

pip install numpy pandas matplotlib seaborn tensorflow scikit-learn

**Motivation**

Solar power generation depends on several environmental and solar-related factors. Variations in temperature, solar radiation, cloud coverage, and other weather conditions influence the amount of electricity generated.

This project aims to:

Understand the relationship between weather conditions and solar power generation.

Identify important parameters influencing solar energy production.

Develop an ANN-based prediction model.

Compare actual and predicted solar power generation.

Explore the application of deep learning in renewable energy forecasting.

**Model Used**

Artificial Neural Network (ANN)

Input Layer: 20 features

Hidden Layer 1: 32 neurons (ReLU)

Hidden Layer 2: 64 neurons (ReLU)

Output Layer: 1 neuron

Optimizer: Adam

Loss Function: Mean Squared Error (MSE)

Epochs: 150

Batch Size: 32

Results

The model was evaluated using RMSE on the original solar power scale.

**Evaluation Metric Result**

Training RMSE-275.90 kW

Testing RMSE-471.43 kW

The model predictions were also visualized against actual solar power generation to examine its performance on training and testing datasets.
