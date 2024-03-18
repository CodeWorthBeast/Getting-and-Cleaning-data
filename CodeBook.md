## Getting and Cleaning Data Course Project Summary

This document describes the data used and the cleaning steps applied for a project in the Johns Hopkins "Getting and Cleaning Data" course. 

**Data Source:**

The data comes from the UCI Machine Learning Repository and focuses on human activity recognition using smartphone sensors.

**Data Description:**

* 30 volunteers (aged 19-48) wore smartphones while performing six activities (walking, walking upstairs/downstairs, sitting, standing, and laying).
* Smartphone sensors (accelerometer and gyroscope) captured movement data.
* The data was split into training (70% of volunteers) and testing (30% of volunteers) sets.

**Data Processing:**

* Sensor data was filtered for noise and divided into overlapping windows. 
* Acceleration data was separated into body motion and gravity components.
* Various features were calculated from each window (time-domain and frequency-domain).

**Data Structure:**

Each record contains:

* Accelerometer data (total and body acceleration)
* Gyroscope data (angular velocity)
* A set of calculated features
* Activity label
* Subject identifier

**Data Cleaning Steps (See Included Instructions):**

A separate document (README.md) details the specific steps taken to clean the data, including:

1. Combining training and testing sets
2. Selecting only mean and standard deviation measurements for each feature
3. Using clear activity names
4. Adding descriptive variable names
5. Creating a new dataset with average features for each activity and subject

This cleaned data is then ready for further analysis.