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

* Student academic records
* Attendance tracking
* Assignment performance
* LMS activity monitoring
* Student wellbeing indicators
* Learning resource engagement
* Demographic and socio-economic information
---


# 🏗️ Data Architecture

This project follows the **Medallion Architecture** approach inside Microsoft Fabric:

![img](https://github.com/nhahub/NHA-4-011/blob/b0d54c56a175503b6b5eaa4abbb87b1031e2a58b/Documents/Workflow.png)

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

# 📊 Available Dataset Columns

The dataset includes the following educational attributes:

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

# 📊 Business Questions Answered by Dashboard

The Power BI dashboard is divided into six analytical areas:

---

# 1️⃣ Academics & Demographics

### Key Analyses

* Department vs Grade
* Scores by Gender
* Age Impact in Same Department
* Hardest and Easiest Subjects

### Insights

* Compare student performance across departments
* Identify gender-based subject strengths
* Detect difficult subjects requiring support
* Analyze age impact on academic achievement

---

# 2️⃣ Socio-Economic Analysis

### Key Analyses

* Parent Education vs Grade
* Income vs Internet Access
* Internet Access vs LMS Usage
* Income Level vs Grade

### Insights

* Analyze socio-economic impact on education
* Detect digital inequality among students
* Measure internet availability impact on LMS engagement

---

# 3️⃣ Wellbeing & Student Habits

### Key Analyses

* Study Hours vs Grade
* Sleep vs Stress
* Stress vs Grades
* Extracurricular Activities vs Study Hours
* Extracurricular Activities vs Stress

### Insights

* Identify optimal study habits
* Measure stress impact on academic performance
* Analyze student mental wellbeing

---

# 4️⃣ LMS Engagement Analytics

### Key Analyses

* LMS Login Frequency vs Grade
* Active Hours vs Scores
* Resource Access vs Grade

### Insights

* Analyze student engagement with learning platforms
* Measure impact of LMS activity on performance
* Evaluate effectiveness of educational resources

---

# 5️⃣ Attendance & Compliance

### Key Analyses

* Academic Attendance vs Grade
* Non-Academic Attendance vs Activities
* Late Assignments vs LMS Logins
* Late Assignments vs Grade
* Stress vs Late Assignments

### Insights

* Measure attendance impact on grades
* Detect procrastination patterns
* Identify behavioral risks affecting academic success

---

# 6️⃣ Subject Correlation Analysis

### Key Analyses

* Math vs Science
* Math vs Computer Science
* Language Skills Correlation
* Assignments vs Final Score

### Insights

* Analyze subject relationships
* Detect STEM capability trends
* Evaluate assignment effectiveness as a performance predictor

---

# 📈 Key Insights Generated

* Students with higher LMS engagement tend to achieve better academic results
* Academic attendance strongly affects final grades
* High stress levels negatively impact performance and assignment completion
* Internet access significantly influences LMS participation
* Continuous assignment performance predicts final academic success
* Balanced extracurricular participation can improve student wellbeing

---

# 🚀 Future Enhancements

* Real-time student monitoring dashboards
* Predictive analytics for dropout detection
* AI-generated academic recommendations
* Automated alerts for at-risk students
* Integration with live LMS platforms
* Advanced NLP educational assistant
