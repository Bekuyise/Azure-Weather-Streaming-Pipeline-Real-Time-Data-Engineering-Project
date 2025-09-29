#  Azure Weather Streaming Pipeline – Real-Time Data Engineering Project(Weather Streaming)

#  Project Overview
This project simulates a real-world scenario where weather and air quality data is ingested, processed, and visualized in real time using Microsoft Azure. Built as an end-to-end cloud-native data engineering pipeline, the solution leverages multiple Azure services for ingestion, streaming, transformation, alerting, and visualization.

The goal is to provide accurate, up-to-the-minute environmental insights that can be used for public safety, environmental monitoring, or operational decision-making.


# Business Problem

### A smart city organization wants to monitor live weather and pollution conditions to:

 Detect and act on hazardous air quality in real time

 Centralize data from  Chennai geographic location

 Deliver live dashboards and alerts for public and internal stakeholders


# Architecture Diagram Solution 



<img width="1200" height="675" alt="Architecture daigram" src="https://github.com/user-attachments/assets/212ea690-93f6-4498-b244-3b02ad32aae4" />


# Tools/technology used

| Component        | Technology                                    |
| ---------------- | --------------------------------------------- |
| Weather Data API | [weatherapi.com](https://www.weatherapi.com/) |
| Ingestion Layer  | Azure Functions (Timer Trigger)               |
| Streaming Layer  | Azure Event Hub                               |
| Processing Layer | Azure Databricks (PySpark)                    |
| Storage Layer    | Azure Kusto DB (ADX)                          |
| Visualization    | Power BI                                      |
| Alerting         | Azure Data Activator + Outlook Email          |
| Security         | Azure Key Vault                               |


#  Dashboard preview 

<img width="637" height="331" alt="image" src="https://github.com/user-attachments/assets/e78d3327-8b5c-40d4-9dd9-45385109439d" />

#  Power BI Dashboard
### The final dashboard provides rich, real-time insights, including:

 Current Weather Conditions

 Air Quality Index (AQI)

 Live Alerts (Weather Warnings)

 3-Day Forecast

 Location-wise Trends and Metrics



#  Key Features Delivered

###  Real-Time Data Ingestion
Automated ingestion from Weather API every 30 seconds using Azure Function
Flattened + enriched JSON data from multiple API endpoints (current, forecast, alerts)

###  Event-Driven Streaming
Data published to Azure Event Hub in structured format
Supports batch and streaming delivery to consumers

###  Streaming ETL & Processing
Databricks notebook processes, validates, and sends enriched data to Kusto DB

structured streaming in micro-batches every 30 seconds

###  Secure Cloud Architecture
All API keys and Event Hub credentials managed via Azure Key Vault


#  Business Impact
### This real-time Azure-based data pipeline enables organizations to:

Make instant decisions on severe weather or pollution events

Replace manual environmental monitoring with automated analytics

Scale across multiple locations for smart city or public health needs

Reduce risk with faster alerting and reliable forecasting








