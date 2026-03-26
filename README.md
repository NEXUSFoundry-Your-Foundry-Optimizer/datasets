# Furnace Anomaly Detection Dataset (Synthetic)

## Overview

This repository contains a **synthetically generated industrial furnace dataset** designed for anomaly detection tasks.
The data simulates real-world furnace sensor readings under **normal operating conditions** and **degradation (fault) scenarios**.

This dataset is generated programmatically and is intended for:

* Machine Learning experiments
* Anomaly Detection research
* Time-series modeling
* Industrial AI applications

## Dataset Description

The dataset consists of two separate CSV files:

### 1. Normal Dataset (`normal_dataset.csv`)

* Represents **healthy furnace operation**
* Used for **model training**
* Generated using stable statistical distributions

### 2. Anomaly Dataset (`anomaly_dataset.csv`)

* Represents **degrading furnace behavior**
* Used for **testing anomaly detection**
* Includes gradual drift and abnormal patterns

## Features

Each record contains the following sensor readings:

| Feature Name    | Description                          |
| --------------- | ------------------------------------ |
| `timestamp`     | Time of reading                      |
| `melt_temp`     | Furnace melting temperature (°C)     |
| `power_kw`      | Power consumption (kW)               |
| `vibration_g`   | Mechanical vibration (g-force)       |
| `lining_health` | Furnace lining condition (0–1 scale) |
| `humidity`      | Ambient humidity (%)                 |
| `ambient_temp`  | Surrounding temperature (°C)         |


## Data Generation Logic

The dataset is generated using two functions:

* **Normal Data**

  * Gaussian distributions around stable means
  * Represents standard industrial conditions

* **Anomaly Data**

  * Gradual degradation introduced over time
  * Increasing temperature, power, vibration
  * Decreasing lining health

This mimics **real-world equipment failure progression**.

## Use Cases

* LSTM Autoencoder anomaly detection
* Predictive maintenance systems
* Industrial IoT analytics
* Time-series forecasting
* Fault detection modeling

## Note

* This is **synthetic data**, not real industrial data
* Designed to closely resemble realistic patterns
* Suitable for experimentation and prototyping
