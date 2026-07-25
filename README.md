 <h1 align="center">🎓 Student 360 — Academic Intelligence Platform</h1>

<p align="center">
A Real-Time Academic Intelligence Platform powered by Data Engineering, Machine Learning, and AI.
</p>

<p align="center">

![Apache Kafka](https://img.shields.io/badge/Apache%20Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=for-the-badge&logo=snowflake&logoColor=white)
![Apache Airflow](https://img.shields.io/badge/Apache%20Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=for-the-badge&logo=dbt&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Microsoft Copilot Studio](https://img.shields.io/badge/Microsoft%20Copilot%20Studio-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)

</p>

<p align="center">
⭐ Real-Time Analytics • Snowflake • Kafka • AI Chatbot • ML Prediction
</p>

---
Project Overview
Student 360 is a real-time academic intelligence platform designed to unify multi-source university data, monitor student performance holistically, and proactively detect dropout risks using machine learning. The platform integrates data engineering, analytics, data science, and AI-powered natural language access into a single end-to-end solution.
> **Institution:** Aditya Engineering College  
> **Domain:** EdTech / Academic Analytics  
> **Type:** Real-Time Data Pipeline + ML + AI Chatbot
---
## 🔴 Problem Statement

Higher education institutions generate vast amounts of data across multiple systems, including academic records, attendance, financial information, examinations, and placements. However, this data is often stored in isolated databases and applications, preventing institutions from obtaining a unified view of student performance.

As a result, universities face several operational and academic challenges:

- Lack of a centralized student data platform
- Difficulty in monitoring academic performance across departments
- Delayed identification of students at risk of academic failure or dropout
- Limited support for data-driven decision-making by faculty and administrators
- Absence of real-time insights for students regarding their academic progress

These fragmented systems lead to reactive interventions rather than proactive student support, ultimately impacting academic outcomes, retention rates, and institutional efficiency.
---
## ✅ Solution

To address these challenges, **Student 360** provides a unified, real-time academic intelligence platform that integrates data engineering, analytics, machine learning, and conversational AI into a single end-to-end solution.

The platform delivers the following capabilities:

- **Real-Time Data Integration** – Ingests student information from multiple sources, including MongoDB and REST APIs, using Apache Kafka for reliable event-driven data streaming.
- **Centralized Data Warehouse** – Consolidates raw and processed data within Snowflake, creating a single source of truth for academic analytics.
- **Data Transformation & Modeling** – Utilizes dbt and SQL to cleanse, validate, and transform raw datasets into standardized analytical models.
- **Workflow Orchestration** – Automates the complete ELT pipeline using Apache Airflow, enabling scheduling, monitoring, and dependency management.
- **Analytics & Reporting** – Generates interactive dashboards and performance insights using SQL and Power BI for faculty, administrators, and management.
- **Machine Learning** – Predicts student performance and identifies potential dropout risks using supervised learning algorithms, enabling proactive academic interventions.
- **AI-Powered Assistant** – Provides a natural language interface through Microsoft Copilot Studio, allowing users to securely access academic information based on role-based permissions.

By combining these technologies into a unified platform, Student 360 enables institutions to make data-driven decisions, improve student retention, and enhance overall academic outcomes.
----
## 🏗️ Solution Architecture

The Student 360 platform follows a modern, event-driven data architecture that integrates multiple data sources, processes data through a scalable ELT pipeline, and delivers analytics, machine learning predictions, and AI-powered insights.

### Architecture Overview



### Architecture Components

| Layer | Technology | Purpose |
|--------|------------|---------|
| **Data Sources** | MongoDB, REST APIs | Collects student, attendance, examination, and academic records |
| **Streaming Layer** | Apache Kafka | Enables real-time event streaming and data ingestion |
| **Data Warehouse** | Snowflake | Stores raw, transformed, and analytics-ready datasets |
| **Transformation Layer** | dbt | Cleanses, validates, and models data using SQL |
| **Orchestration Layer** | Apache Airflow | Schedules, monitors, and automates ELT workflows |
| **Analytics Layer** | SQL, Power BI | Provides dashboards and performance insights |
| **Machine Learning Layer** | Python, Scikit-learn | Predicts student performance and dropout risk |
| **AI Layer** | Microsoft Copilot Studio | Enables secure natural language access to student information |
---
## 🛠️ Technology Stack

The Student 360 platform leverages a modern data engineering and AI ecosystem to support real-time data integration, analytics, machine learning, and conversational AI.

| Category                      | Technology               | Description                                                                                                              |
| ----------------------------- | ------------------------ | ------------------------------------------------------------------------------------------------------------------------ |
| **Programming Language**      | Python 3.10+             | Core language used for data ingestion, pipeline development, machine learning, and automation.                           |
| **Data Sources**              | MongoDB, REST APIs       | Collects student records, attendance, examination results, and academic data from multiple systems.                      |
| **Event Streaming**           | Apache Kafka             | Enables reliable, real-time data ingestion and event-driven communication between source systems and the data warehouse. |
| **Cloud Data Warehouse**      | Snowflake                | Centralized repository for storing raw, transformed, and analytics-ready datasets.                                       |
| **Data Transformation**       | dbt (Data Build Tool)    | Performs SQL-based data transformation, testing, documentation, and data modeling.                                       |
| **Workflow Orchestration**    | Apache Airflow           | Automates, schedules, and monitors end-to-end ELT workflows using DAGs.                                                  |
| **Analytics & Visualization** | SQL, Power BI            | Generates interactive dashboards, KPIs, and analytical reports for stakeholders.                                         |
| **Machine Learning**          | Python, Scikit-learn     | Builds predictive models for student performance analysis and dropout risk prediction.                                   |
| **AI Assistant**              | Microsoft Copilot Studio | Provides a secure natural language interface for students and administrators with role-based access.                     |
| **Version Control**           | Git & GitHub             | Manages source code, collaboration, and version history throughout the development lifecycle.                            |
-----
## 📁 Project Structure

```text
student360/
│
├── kafka/                          # Real-time data ingestion
│   ├── mongodb_producer.py
│   ├── mongodb_consumer.py
│   ├── api_producer.py
│   └── api_consumer.py
│
├── dbt/                            # Data transformation layer
│   ├── dbt_project.yml
│   ├── profiles.yml
│   └── models/
│       ├── staging/
│       ├── intermediate/
│       └── marts/
│
├── airflow/
│   └── dags/
│       └── student_pipeline_dag.py
│
├── snowflake/                      # Database objects
│   ├── create_tables.sql
│   ├── views.sql
│   └── procedures.sql
│
├── ml/                             # Machine Learning modules
│   ├── feature_engineering.py
│   ├── dropout_prediction.py
│   └── model_evaluation.py
│
├── chatbot/                        # Microsoft Copilot Studio
│   ├── prompts/
│   ├── power_automate/
│   └── README.md
│
├── powerbi/                        # Dashboard files
│   └── Student360.pbix
│
├── docs/                           # Project documentation
│   ├── architecture.png
│   ├── workflow.png
│   └── Project_Report.pdf
│
├── assets/                         # README images
│   ├── banner.png
│   ├── dashboard.png
│   ├── architecture.png
│   └── demo.gif
│
├── config/
│   ├── .env.example
│   └── config.yaml
│
├── requirements.txt
├── .gitignore
├── LICENSE
└── README.md
```
⚙️ Setup & Installation
Prerequisites
Python 3.10+
Apache Kafka (local or cloud)
Snowflake account
Apache Airflow
dbt-snowflake installed
1. Clone the repository
```bash
git clone https://github.com/your-username/student360.git
cd student360
```
2. Install Python dependencies
```bash
pip install -r requirements.txt
```
3. Configure environment variables
```bash
cp .env.example .env
# Edit .env with your Snowflake, Kafka, and MongoDB credentials
```
4. Run Kafka producers
```bash
# Terminal 1 - MongoDB producer
python kafka/mongodb_producer.py

# Terminal 2 - API producer
python kafka/api_producer.py
```
5. Run Kafka consumers
```bash
# Terminal 3 - MongoDB consumer
python kafka/mongodb_consumer.py

# Terminal 4 - API consumer
python kafka/api_consumer.py
```
6. Run dbt transformations
```bash
cd dbt
dbt run
dbt test
```
7. Start Airflow
```bash
airflow db init
airflow scheduler &
airflow webserver
```
---
## 🗄️ Snowflake Data Model

The Student 360 platform organizes data using a layered architecture in Snowflake, separating raw ingestion, transformed datasets, and analytics-ready models. This approach ensures data consistency, scalability, and simplified reporting.

---

### **STG_MONGODB** *(Raw Student Profile Data)*

This staging table stores student profile information ingested directly from MongoDB.

| Column       | Data Type | Description                                |
| ------------ | --------- | ------------------------------------------ |
| `STUDENT_ID` | VARCHAR   | Unique identifier assigned to each student |
| `NAME`       | VARCHAR   | Full name of the student                   |
| `DEPARTMENT` | VARCHAR   | Academic department or branch              |
| `YEAR`       | NUMBER    | Current year of study                      |
| `CGPA`       | FLOAT     | Cumulative Grade Point Average             |
| `BACKLOGS`   | NUMBER    | Total number of active backlogs            |

---

### **STG_API** *(Raw Attendance & Examination Data)*

This staging table stores attendance and examination data received from external REST APIs.

| Column           | Data Type | Description                            |
| ---------------- | --------- | -------------------------------------- |
| `STUDENT_ID`     | VARCHAR   | Unique student identifier              |
| `SUBJECT`        | VARCHAR   | Subject or course name                 |
| `MARKS`          | FLOAT     | Marks obtained in the examination      |
| `ATTENDANCE_PCT` | FLOAT     | Attendance percentage                  |
| `EXAM_TYPE`      | VARCHAR   | Examination type (Internal / External) |

---

### **STUDENT_UNIFIED** *(Analytics-Ready Student Dataset)*

This curated table combines data from multiple sources using dbt models and serves as the primary dataset for analytics, reporting, machine learning, and AI-powered applications.

| Column               | Data Type | Description                                         |
| -------------------- | --------- | --------------------------------------------------- |
| `STUDENT_ID`         | VARCHAR   | Unique student identifier                           |
| `NAME`               | VARCHAR   | Student name                                        |
| `DEPARTMENT`         | VARCHAR   | Academic department                                 |
| `CGPA`               | FLOAT     | Overall cumulative GPA                              |
| `AVG_MARKS`          | FLOAT     | Average marks across all subjects                   |
| `ATTENDANCE_PCT`     | FLOAT     | Overall attendance percentage                       |
| `BACKLOGS`           | NUMBER    | Total number of active backlogs                     |
| `DROPOUT_RISK_SCORE` | FLOAT     | Machine learning-generated risk score *(0.0 – 1.0)* |
| `RISK_CATEGORY`      | VARCHAR   | Risk classification *(LOW, MEDIUM, HIGH)*           |

---

### 📊 Data Flow

```text
MongoDB
      │
      ▼
 STG_MONGODB
      │
REST APIs
      │
      ▼
   STG_API
      │
      ▼
dbt Transformations
      │
      ▼
STUDENT_UNIFIED
      │
      ├── Power BI Dashboards
      ├── Machine Learning Models
      └── Microsoft Copilot Studio
```
🤖 Machine Learning — Dropout Risk Prediction
Model Details
Algorithm: Random Forest Classifier + Logistic Regression (ensemble)
Target Variable: Dropout Risk (Low / Medium / High)
Features Used:
CGPA
Attendance percentage
Number of backlogs
Average marks
Department
Academic year
Model Performance
Metric	Score
Accuracy	87%
Precision	85%
Recall	83%
F1 Score	84%
---
💬 AI Chatbot — Microsoft Copilot Studio
The chatbot is built using Microsoft Copilot Studio integrated with Snowflake via Power Automate.
Role-Based Access Control
Role	Access
Admin	View all students' marks, attendance, predictions, risk scores
Student	View only their own marks, attendance, and predictions
Sample Conversations
```
Student: "What are my marks?"
Bot: "Here are your marks: Math 85, Science 90, English 78. Overall Grade: B+"

Student: "What is my attendance?"
Bot: "Your attendance this semester is 87%. You have 6 absences."

Student: "Will I pass this semester?"
Bot: "Based on your performance, your predicted outcome is: PASS (82% probability)"

Admin: "Show me all at-risk students"
Bot: "15 students are currently HIGH risk. Top 3: [Student A, Student B, Student C]"
```
---
📊 Analytics Dashboards (Power BI)
The platform provides the following dashboards:
Student Performance Dashboard — Individual marks, CGPA trend, subject-wise analysis
Attendance Analytics — Department-wise attendance heatmap, absentee alerts
Dropout Risk Dashboard — Risk score distribution, high-risk student list
Placement Readiness — CGPA vs placement eligibility analysis
Department Overview — Comparative performance across departments
---
🔄 Apache Airflow — Pipeline Orchestration
The main DAG (`student_pipeline_dag.py`) runs the following tasks in sequence:
```
start
  │
  ├── extract_mongodb_data
  │       │
  │       └── kafka_produce_mongodb
  │               │
  │               └── kafka_consume_mongodb → load_to_snowflake_stg1
  │
  ├── extract_api_data
  │       │
  │       └── kafka_produce_api
  │               │
  │               └── kafka_consume_api → load_to_snowflake_stg2
  │
  └── [after both above complete]
          │
          └── run_dbt_transformations
                  │
                  └── run_ml_predictions
                          │
                          └── update_dropout_risk_scores → end
```
Schedule: Runs every 6 hours automatically
---
🚀 Future Scope
Mobile App — React Native app for students to access their data on mobile
Real-time Alerts — SMS/email alerts to faculty when a student becomes high-risk
Parent Portal — Secure parent access to their child's academic data
Advanced ML — Deep learning models for more accurate predictions
Multi-institution Support — Scale platform across multiple universities
Integration with ERP — Connect with college ERP systems (fees, hostel, library)
Recommendation Engine — AI-powered subject and career recommendations
---
## 👥 Project Team

| Team Member                             | Primary Responsibility                                                                                                                                                                             |
| --------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **VARRE KAVYA SRI**                     | **Solution Architecture, AI Integration, Microsoft Copilot Studio, Power Automate Integration, Conversational AI Development, System Integration, Technical Documentation & Project Coordination** |
| **Billakurthi Varshitha**               | Real-Time Data Engineering, Apache Kafka Pipelines, Snowflake Data Ingestion                                                                                                                       |
| **Silarapu Varshini Satyapriya**        | Data Transformation, dbt Modeling, SQL Development, Data Quality Validation                                                                                                                        |
| **Budamparthi Jyothsna Vijaya Lakshmi** | Machine Learning Model Development, Feature Engineering, Dropout Risk Prediction                                                                                                                   |
| **Pilli Mounika Sai Sruthi**            | Business Intelligence, Power BI Dashboards, Data Visualization & Analytics                                                                                                                         |

📄 License
This project is developed as part of an academic project at Aditya Engineering College.
---
🙏 Acknowledgements
Apache Kafka, Snowflake, dbt, Apache Airflow open-source communities
Microsoft Copilot Studio documentation
Scikit-learn Machine Learning library
Our faculty mentors and project guides at Aditya Engineering College
