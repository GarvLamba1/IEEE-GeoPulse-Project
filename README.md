# IEEE-GeoPulse-Project
AI-Based Solar Site Viability Detection Using Environmental Sensors

This project uses environmental sensor data and machine learning to determine whether a location is suitable for installing solar panels. By analyzing temperature, humidity, and light intensity data collected from sensors, the system classifies areas as suitable, borderline, or unsuitable for renewable energy installation.

The goal of this project is to demonstrate how AI and IoT sensor data can be combined to support smarter decisions about renewable energy placement.

Project Overview

Environmental sensors collect real-world data including:

Temperature (°C)

Humidity (%)

Light intensity

This data is processed and labeled using threshold-based rules and then used to train a neural network model that predicts solar installation viability.

The system can automatically classify a location into three categories:

Suitable – High solar potential

Borderline – Moderate solar potential

Unsuitable – Low solar potential

Features

Sensor data processing from XML feeds

Automatic dataset generation

Threshold-based baseline classifier

Neural network model trained using TensorFlow / PyTorch

Dataset compatible with Edge Impulse

Model evaluation using precision, recall, and confusion matrices

Technologies Used

Python

TensorFlow / PyTorch

Pandas

NumPy

Edge Impulse

Environmental Sensors (BH1750, DHT11)

Dataset

The dataset contains sensor readings including:

Temperature

Humidity

Light intensity

Each data sample is labeled based on environmental thresholds to determine solar suitability.

Repository Structure
dataset/
 ├── renewable_energy_dataset.csv
 ├── edge_impulse_train.csv
 ├── edge_impulse_inference.csv

models/
 ├── solar_viability_model.h5

scripts/
 ├── dataset_builder.py
 ├── threshold_classifier.py
 ├── train_model.py
Model Performance

The neural network model achieved high accuracy in identifying clear cases of solar viability. However, performance on borderline cases was limited due to class imbalance in the dataset, highlighting the need for more mid-range environmental samples.

Future Improvements

Larger and more balanced dataset

Additional environmental features (solar irradiance, cloud coverage, location)

Real-time data processing

Integration with mapping systems to visualize optimal renewable energy locations

Goal

The ultimate goal is to build an intelligent system that helps identify optimal locations for renewable energy installations using real-time environmental data.
