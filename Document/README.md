[English](./README.md)|[简体中文](./README.ch-zh.md)

# **Streaming Power Load Forecasting Framework**

## **1 Project Introduction**

### **1.1 Background**

As power systems move toward intelligence and decarbonization, power load forecasting plays an increasingly important role in grid operation and planning. High-accuracy forecasting not only enables utilities to balance supply and demand and reduce system losses, but also enhances the integration and utilization efficiency of renewable energy sources, thereby supporting the sustainable and low-carbon development of modern power systems.

However, the operational environment of modern grids has become increasingly complex. The large-scale deployment of smart meters, sensors, and IoT devices has resulted in massive, high-frequency, and heterogeneous power data across spatial and temporal dimensions. Meanwhile, the volatility of renewable generation (e.g., solar and wind power) and the growing penetration of distributed energy resources pose higher challenges to prediction accuracy and real-time responsiveness. Traditional forecasting approaches based on time series analysis or linear regression have shown limitations in addressing such dynamic and time-varying characteristics of modern power systems.

In this context, machine learning techniques offer new opportunities for power load forecasting. By integrating heterogeneous data sources such as smart meter readings, meteorological conditions, building attributes, and user behavior, machine learning models are capable of capturing complex nonlinear relationships and multi-scale fluctuations, providing an analytical foundation for intelligent dispatching, demand response, and energy storage optimization.

### **1.2 Project Overview**

This project is based on real-world power load data collected in 2022 from a district in Melbourne, Australia, provided by a local power company. Combined with meteorological and building information, the goal is to develop a high-accuracy and scalable streaming power load forecasting framework to support real-time decision-making and dynamic scheduling in smart grids.

The project is implemented in two phases: the first focuses on model development and validation, and the second on system deployment and streaming prediction.

### **1.2.1 Phase I: Model Development and Validation**

The first phase focuses on developing a high-performance power load forecasting model. Leveraging the Spark distributed computing framework, multi-source data are processed and transformed in parallel to extract relevant features.

The dataset consists of three main components:

1. Real-time power measurements from smart meters, representing the temporal dynamics of user load;
2. Meteorological data (e.g., temperature, humidity, and wind speed), reflecting the impact of external environmental factors on energy consumption;
3. Building information (e.g., building type, usage, and area), describing heterogeneity among different user groups.

Two ensemble learning algorithms—Random Forest (RF) and Gradient Boosting Tree (GBT)—are employed to analyze feature importance and capture nonlinear relationships between variables, thereby uncovering the coupling effects of climatic and structural factors on load variation.

Model performance is evaluated through cross-validation and multiple metrics, including the Root Mean Squared Logarithmic Error (RMSLE), to ensure model stability and generalization, forming a robust foundation for real-time prediction in the next phase.

### **1.2.2 Phase II: System Deployment and Streaming Prediction**
The second phase focuses on real-time implementation and system-level deployment.

Based on the Kafka streaming framework, a dynamic pipeline is established to integrate data ingestion, model inference, and prediction output, enabling end-to-end automation from data acquisition to feedback delivery.

Kafka’s message queue mechanism ensures decoupling and buffering of high-frequency data streams, maintaining efficient system operation under concurrent workloads.

In parallel, Spark Streaming is employed to process real-time data continuously, allowing the model to produce updated predictions that can be instantly fed into the utility company’s decision-making system.
This phase marks the transition from offline model training to online prediction, providing both algorithmic and infrastructural support for intelligent grid dispatching, demand response, and energy optimization.

## **2 Project Progress**

- [x] Model Development and Validation
- [ ] System Deployment and Streaming Prediction (In Progress)