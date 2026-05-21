# NHA-4-11
# 📊 Education system montoring & AI Chatbot Solution on Microsoft Fabric

This project demonstrates the design and implementation of a modern **Education Monitoring System** using **Microsoft Fabric** and **Power BI**, simulating real-world educational analytics, student performance tracking, and AI-powered academic assistance.

The solution transforms raw educational data into a scalable, analytics-ready lakehouse platform that enables schools and educational institutions to monitor student performance, attendance, LMS engagement, wellbeing, and socio-economic factors through interactive dashboards and AI-driven insights.

The project follows industry best practices including **Medallion Architecture (Bronze → Silver → Gold)**, data modeling, educational analytics, and Retrieval-Augmented Generation (**RAG**) for intelligent chatbot interactions.

---

# 📖 Project Overview

This project covers the complete educational data lifecycle:

* **Data Architecture** — Building a scalable educational lakehouse using Medallion Architecture
* **ETL Pipelines** — Processing and transforming educational datasets using PySpark & SQL
* **Data Modeling** — Designing analytical models for student monitoring and reporting
* **Data Quality** — Cleaning missing values, correcting inconsistencies, and standardizing data
* **Analytics & Reporting** — Developing interactive dashboards in Power BI
* **AI Chatbot (RAG System)** — Building an intelligent educational assistant connected to educational books and student databases

---

# 🛠️ Tools & Technologies

| Category                  | Tools                                               |
| --------------------------| --------------------------------------------------- |
| **Data Platform**         | Microsoft Fabric                                    |
| **Storage**               | OneLake / Lakehouse                                 |
| **Processing**            | Apache Spark, PySpark                               |
| **Languages**             | Python, SQL                                         |
| **Visualization**         | Power BI                                            |
| **AI & NLP**              | RAG (Retrieval-Augmented Generation), Vector Search |
| **statistical operations**| pandas library                                      |
| **Version Control**       | Git / GitHub                                        |

---

# 🎯 Project Objectives

This project demonstrates both **Data Engineering** and **Educational Analytics** capabilities.

## Data Engineering Goals

* Build a scalable educational lakehouse using Microsoft Fabric
* Ingest educational datasets into Bronze Layer
* Transform and validate data using PySpark and SQL
* Apply data quality checks and business rules
* Create analytical models optimized for Power BI reporting
* Implement Medallion Architecture best practices

---

## Analytics Goals

* Monitor student academic performance
* Analyze attendance and engagement patterns
* Detect students at academic risk
* Analyze LMS engagement and learning behavior
* Evaluate socio-economic impact on education
* Support data-driven educational decision-making

---

# 📁 About Dataset

The dataset represents a complete educational monitoring environment containing:


| Category                       | Columns                                                                                              |
| ------------------------------ | ---------------------------------------------------------------------------------------------------- |
| **Student Information**        | Student_ID, First_Name, Last_Name, Email, Gender, Age                                                |
| **Academic Data**              | Department, Grade, Total_Avg, last_score                                                             |
| **Subject Scores**             | Math_Score, Science_Score, English_Score, French_Score, Social_Studies_Score, Computer_Science_Score |
| **Assignments**                | assi_Math, assi_Science, assi_English, assi_French, assi_Social_Studie, assi_computer_science        |
| **Attendance**                 | academic_attendance, non_academic_attendance                                                         |
| **LMS Analytics**              | lms_login_freq_per_day, lms_active_avg_hrs, resource_access_avg_hrs                                  |
| **Student Habits & Wellbeing** | Study_Hours_per_Week, Stress_Level, Stress_Level_1_10, Sleep_Hours_per_Night                         |
| **Socio-Economic Data**        | Parent_Education_Level, Family_Income_Level, Internet_Access_at_Home                                 |
| **Activities**                 | Extracurricular_Activities                                                                           |
| **Assignments & Compliance**   | assi_late                                                                                            |

---


# 🏗️ Data Architecture

This project follows the **Medallion Architecture** approach inside Microsoft Fabric:

![img](https://github.com/nhahub/NHA-4-011/blob/52b259a4b8a26fe643c58cac4cfacd847a13ec9a/Documents/workflow.jpeg)

### Bronze Layer

Contains raw educational records including:

* Student profiles
* Subject scores
* Assignments
* Attendance records
* LMS logs
* Wellbeing indicators

### Silver Layer

Includes:

* Data cleansing
* Standardized naming conventions
* Null value handling
* Data quality validation
* Feature engineering

### Gold Layer

Contains:

* Fact and dimension tables
* Educational KPIs
* Student risk indicators
* Dashboard-ready analytical models

---


# 🤖 AI Chatbot (RAG + Pandas Analytical System)

The project includes an intelligent AI-powered chatbot built using a **Retrieval-Augmented Generation (RAG)** architecture combined with **Pandas-based educational data analysis**.

## Chatbot Features

* Connected to educational books and learning materials
* Retrieves educational content using vector search
* Answers academic and subject-related questions
* Connected directly to the educational database
* Performs educational data analysis and statistics using Pandas
* Generates personalized educational insights and recommendations

## Chatbot Capabilities

* Explain educational concepts from textbooks
* Answer subject-specific questions
* Analyze student performance trends
* Perform statistical analysis on student data using Pandas
* Generate insights from educational datasets
* Recommend educational resources
* Detect weak subjects and learning gaps
* Provide personalized academic guidance

## Hybrid Query Routing Mechanism

The chatbot uses a hybrid routing mechanism to determine the appropriate processing method based on the user's query.

* Educational and textbook-related questions are routed to the **RAG pipeline**, where relevant content is retrieved from embedded PDF documents using vector similarity search.
* Analytical and database-related questions are routed to a **Pandas DataFrame Agent**, enabling the chatbot to perform calculations, statistics, filtering, aggregation, and educational data analysis directly on student datasets.

This hybrid architecture allows the chatbot to combine:
* Semantic educational retrieval from books and learning materials
* Intelligent data analysis and educational analytics using Pandas

As a result, the system can answer both:
* Conceptual educational questions
* Data-driven analytical questions
---

# 📊 Business Questions Answered by Dashboard

The Power BI dashboard is divided into six analytical areas:

---
## Research Questions

1. **How do academic and demographic factors** (department, gender, age, and subject difficulty) influence student performance?

2. **How do socio-economic factors** such as family income, parent education, and internet access affect academic achievement and LMS engagement?

3. **How do student wellbeing and study habits** including study hours, sleep quality, stress levels, and extracurricular activities impact academic success?

4. **How does LMS engagement** (login frequency, active hours, and resource access) contribute to student performance and learning outcomes?

5. **How do attendance and behavioral patterns** such as academic attendance, late assignments, and procrastination affect student achievement?

6. **What correlations exist between subjects and assessments** such as Math, Science, Computer Science, assignments, and final scores?


---

# 🚀 Future Enhancements

* Real-time student monitoring dashboards
* Predictive analytics for dropout detection
* AI-generated academic recommendations
* Automated alerts for at-risk students
* Integration with live LMS platforms
* Advanced NLP educational assistant
