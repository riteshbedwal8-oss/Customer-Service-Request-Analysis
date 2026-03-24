# Customer-Service-Request-Analysis
Project 1

DESCRIPTION

Background of Problem Statement :
NYC 311 is a centralized service that provides citizens with easy access to non-emergency government services and information. It handles thousands of daily requests related to issues such as noise complaints, illegal parking, public safety, and infrastructure problems. These requests are routed to appropriate departments, resolved, and then marked as closed. Analyzing this data can help improve service efficiency, identify problem areas, and support better decision-making.

---

Problem Objective :
The objective of this project is to perform a comprehensive analysis of New York City 311 service request data. The focus is on applying data wrangling, exploratory data analysis, visualization, and statistical techniques to understand complaint patterns, response times, and key influencing factors.

Domain: Customer Service / Data Analytics

---

Analysis Tasks to be performed:

* Import and explore the NYC 311 service request dataset
* Convert "Created Date" and "Closed Date" into datetime format
* Create a new feature **"Request_Closing_Time"** to measure response time
* Perform data cleaning by handling missing values and removing invalid records
* Analyze complaint distribution across different cities
* Identify the **top 10 most frequent complaint types**
* Visualize complaint patterns using bar charts, scatter plots, and hexbin plots
* Analyze complaint concentration in specific locations (e.g., Brooklyn)
* Create a cross-tabulation of complaint types across cities
* Sort complaint types based on average response time
* Perform statistical analysis using **Kruskal-Wallis Test**
* Interpret p-values to determine significant variables

---

Statistical Analysis:

* **Null Hypothesis (H0):** Average response time is the same across all complaint types
* **Alternate Hypothesis (H1):** Average response time differs across complaint types

A Kruskal-Wallis test was performed to evaluate these hypotheses.

* Obtained p-value: **< 0.05**
* Decision: **Reject the Null Hypothesis (H0)**

Conclusion:
There is a statistically significant difference in response times across different complaint types, indicating that complaint type is an important factor affecting service efficiency.

---

Dataset Description :

The dataset consists of more than 360,000 records and includes the following key fields:

* Unique Key – Unique identifier for each complaint
* Created Date – Date and time when the complaint was raised
* Closed Date – Date and time when the complaint was resolved
* Agency & Agency Name – Department handling the complaint
* Complaint Type – Type/category of complaint
* Descriptor – Detailed description of the complaint
* Location Type – Type of location (residential, commercial, etc.)
* Incident Zip & Address – Location details
* City & Borough – Geographic information
* Status – Status of the complaint (closed/pending)
* Latitude & Longitude – Geographic coordinates
* Request_Closing_Time – Time taken to resolve the complaint (derived feature)

Additional fields include various location, transportation, and infrastructure-related attributes, many of which contain missing or optional data.

---

Conclusion :

This project demonstrates the use of data analysis techniques to extract meaningful insights from real-world service request data. The findings highlight key complaint trends, geographic patterns, and variations in response time, which can help improve operational efficiency and enhance public service delivery.

---

Key Insights :

* Complaint volume is highest in major cities such as New York, Brooklyn, and Queens
* A small number of complaint types dominate the dataset
* Complaint distribution varies across different locations
* Response time differs significantly across complaint categories
* Certain areas show high complaint density, indicating potential hotspots
