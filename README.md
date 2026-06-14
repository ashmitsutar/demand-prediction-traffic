GridLock Traffic Demand Prediction
Overview

This project was developed for the GridLock Traffic Demand Forecasting Challenge, where the objective was to accurately predict traffic demand using tabular data collected from multiple geographical locations, road types, weather conditions, and temporal factors.

The solution combines extensive feature engineering with ensemble machine learning techniques to capture complex traffic patterns and improve prediction accuracy.

Problem Statement

Predict traffic demand based on:

Geographical location
Road characteristics
Weather conditions
Vehicle information
Temporal patterns

The challenge required building a robust model capable of generalizing across diverse traffic scenarios.

Dataset

The dataset consists of traffic-related records containing:

Geohash locations
Road types
Number of lanes
Weather conditions
Temperature
Vehicle information
Timestamp-based features

The target variable is traffic demand.

Feature Engineering

A total of 37 features were utilized, including:

Core Features
Geohash
Road Type
Number of Lanes
Temperature
Weather
Large Vehicles
Landmarks
Day
Temporal Features
Hour
Minute
Hour Sin/Cos Encoding
Minute Sin/Cos Encoding
Peak Time Indicator
Time Blocks
Target Encoding Features
Geohash Target Encoding
Geo Target Hour
Geo Target Frequency
Geo Target Road
Geo Target Temperature
Interaction Features
Lanes × Temperature
Temperature × Hour
GeoHash × Hour
GeoHash × Road Type
Road Pressure
Road Density
Road Capacity Time

These engineered features were designed to capture spatial, temporal, and environmental traffic behavior.

Model Architecture
LightGBM

Used for:

Fast training
Handling large tabular datasets
Capturing complex feature interactions
CatBoost

Used for:

Robust categorical feature handling
Better generalization
Reduced overfitting
Ensemble Learning

Predictions from LightGBM and CatBoost were combined to leverage the strengths of both models and improve overall performance.

Technologies Used
Python
Pandas
NumPy
LightGBM
CatBoost
Scikit-Learn
Matplotlib
Key Contributions
Engineered 37 meaningful features from raw traffic data.
Built an ensemble of LightGBM and CatBoost models.
Captured temporal, spatial, and environmental demand patterns.
Applied target encoding, cyclic encoding, and interaction-based feature engineering.
Improved forecasting performance through ensemble learning.
Results

The final solution successfully modeled traffic demand patterns by combining:

Advanced feature engineering
Target encoding
Ensemble learning
Gradient boosting techniques

resulting in a robust traffic demand forecasting pipeline.

Author

Ashmit Sutar
B.Tech Artificial Intelligence & Machine Learning
Machine Learning Enthusiast
