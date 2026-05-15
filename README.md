🏥 Healthcare Wearable Analytics Lakehouse
📌 Project Overview

This project demonstrates the design and implementation of a modern healthcare analytics pipeline using Medallion Architecture in Databricks.

The solution processes wearable sensor and ECG data from multiple subjects performing physical activities, transforming raw IoT healthcare data into business-ready analytics and KPI dashboards.

The project was developed using the Databricks Free Edition environment with PySpark and Delta Lake technologies.

🚀 Business Problem

Healthcare and wearable technology companies generate large volumes of sensor data from smart devices such as:

Smartwatches
Fitness trackers
ECG monitors
Remote patient monitoring systems

The challenge is transforming raw sensor data into structured, reliable, and analytics-ready datasets for:

Patient monitoring
Activity recognition
Healthcare analytics
Biometrics analysis
Operational dashboards

This project simulates a modern health-tech analytics platform capable of ingesting, transforming, and analyzing wearable sensor data.

🧠 Dataset Information

Dataset used:

mHealth Dataset — UCI Machine Learning Repository

The dataset contains body motion and ECG recordings from 10 subjects performing multiple physical activities.

Activities Included
Standing
Sitting
Lying Down
Walking
Climbing Stairs
Waist Bends
Arm Elevation
Knee Bends
Cycling
Jogging
Running
Jumping
Sensor Data Included
Accelerometer
Gyroscope
Magnetometer
ECG signals
🏗️ Architecture
Medallion Architecture
Wearable Sensors
       ↓
Bronze Layer
       ↓
Silver Layer
       ↓
Gold Analytics
       ↓
Dashboards / KPIs
⚙️ Technologies Used
Technology	Purpose
Databricks	Data engineering platform
PySpark	Distributed data processing
Delta Lake	Modern lakehouse storage
Python	Data transformations
SQL Analytics	KPI generation
Medallion Architecture	Data modeling strategy
🥉 Bronze Layer

The Bronze Layer stores raw ingested healthcare data.

Features
Multi-file ingestion
Raw wearable sensor data
Metadata tracking
Source file tracking
Ingestion timestamps
Subject ID extraction
Key Columns Added
source_file
ingestion_timestamp
subject_id
🥈 Silver Layer

The Silver Layer performs data cleaning and standardization.

Transformations
Null handling
Data quality validation
Activity label mapping
Type casting
Data normalization
Derived ECG metrics
Example Derived Column
ecg_signal_avg
🥇 Gold Layer

The Gold Layer generates analytics-ready datasets and KPIs.

KPIs Created
Average movement intensity
Average ECG signal
Activity intensity classification
User activity analytics
Total activity records
Example Analytics
Running activities show higher movement intensity
Sitting activities show lower biometric activity
ECG averages vary by physical activity
📊 Dashboard & Analytics

The project includes visual analytics generated directly in Databricks.

Visualizations
Average ECG signal by activity
Movement intensity by activity
Activity distribution
Subject-level analytics
📂 Project Structure
project/
│
├── 01_bronze_ingestion
├── 02_silver_transformation
├── 03_gold_analytics
├── architecture_diagram.png
├── screenshots/
│   ├── actividades_mas_realizadaa.png
│   ├── Average_ECG_Signal_by_Activity.png
│   └── movement_intensity.png
│
└── README.md
📸 Project Visualizations
Average ECG Signal by Activity




Movement Intensity Analytics




Most Performed Activities




📈 Key Data Engineering Concepts Demonstrated
Medallion Architecture
Delta Lake
Data Lineage
Metadata Tracking
Healthcare Analytics
IoT Data Processing
KPI Aggregation
Distributed Processing with PySpark
Data Quality Validation
💡 Business Value

This project demonstrates how wearable healthcare data can be transformed into meaningful analytics for:

Remote patient monitoring
Fitness analytics
Health-tech platforms
Activity recognition systems
Biometrics analytics
Executive reporting
🧪 Future Improvements

Potential future enhancements:

Real-time streaming ingestion
Machine learning activity prediction
Anomaly detection
Patient risk scoring
Advanced dashboards
Cloud deployment
Data orchestration pipelines
👨‍💻 Author

Kevin Sterling

Aspiring Data Engineer focused on:

Data Engineering
Databricks
PySpark
Healthcare Analytics
Modern Lakehouse Architectures
⭐ Final Notes

This project was developed as part of a hands-on learning journey in modern data engineering using Databricks and healthcare IoT datasets.

The objective was not only to build ETL pipelines, but also to simulate real-world enterprise analytics workflows using industry-standard architecture and tools.
