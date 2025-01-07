# From-GCS-to-BigQuery


**Global Health Data Analytics Solution**

The Medical Research Team receives a comprehensive global health statistics file containing disease data for all countries. Due to the sensitive nature of the data, there are strict privacy and access control requirements: each country’s Health Minister should have access only to their respective country's medical data. Additionally, they need the ability to analyze and gain insights into diseases for which no treatment or vaccination is currently available.

The data is currently provided as a single file containing over 1 million records, covering a broad spectrum of diseases across various countries. This presents significant challenges:

Security and confidentiality: The data must be restricted and not shared with unauthorized individuals or countries.

Data complexity: The large CSV file is inefficient for analysis due to its size, and extracting meaningful insights from such a dataset is complex and time-consuming.

**Challenges**

Data Confidentiality: Sharing a single, large file with all the stakeholders is not feasible because of the sensitive nature of the data.

Data Volume: The file contains over a million records, making analysis slow and inefficient, particularly when working with large datasets.

Lack of Segregation: Currently, there is no way to efficiently restrict access to each country’s specific data, making it harder to maintain privacy while enabling analysis.

![image](https://github.com/user-attachments/assets/79a6ba39-6b1d-45d3-a6c1-985f71bd62db)

**Objective**

The objective of this project is to develop a robust data analytics solution to securely manage and analyze the disease data. The solution must ensure:


Restricted Access: Each Health Minister should be granted access only to data from their own country, protecting sensitive information.

Efficient Analysis: The solution should streamline the process of analyzing the data, focusing on diseases for which no treatment or vaccination is currently available, thus facilitating decision-making and research.

Scalable and Secure Infrastructure: The data should be stored and processed securely using cloud technologies like Google Cloud Platform (GCP), with access control mechanisms ensuring that sensitive information is handled properly.

Looker Reporting: Use Looker for data visualization and reporting, enabling interactive dashboards and reports for the Health Ministers to monitor and analyze country-specific disease data.

**Solution Approach**

To meet these objectives, the project will involve:


**Data Storage and Management:
**

Store the dataset in a secure cloud environment like Google Cloud Storage (GCS) and BigQuery, ensuring fast, scalable, and secure data storage.

Implement row-level security in BigQuery to ensure that each country’s Health Minister can only view the data for their respective country.

**Data Transformation:**

Create a data pipeline to extract, load, and transform (ELT) the data. This will involve filtering out irrelevant data and creating country-specific tables in BigQuery.

Use Apache Airflow for orchestration and automation of the ETL processes to make the pipeline efficient and scalable.

**Data Access Control:**

Implement role-based access control (RBAC) to ensure that each Health Minister can only access their own country’s data.
Use Google Cloud IAM (Identity and Access Management) and BigQuery permissions to ensure secure and controlled access.

**Looker Reporting:**

Set up Looker to enable Health Ministers to explore the data through interactive dashboards.
Provide the ability to filter and visualize data on diseases without available treatments or vaccines, empowering the Health Ministers with actionable insights.

**Key Features**

Data Security: Role-based access control to ensure confidentiality of sensitive health data.

Efficient Data Handling: A cloud-based, scalable data infrastructure using Google Cloud Platform (GCP) and BigQuery for fast processing of large datasets.

Data Visualization: Interactive dashboards using Looker, allowing Health Ministers to drill down into country-specific disease data.

Automation: The pipeline is fully automated using Apache Airflow, reducing the complexity and manual effort involved in data processing.

Analytics on Treatment/Vaccination Gaps: Focused analysis on diseases with no available treatments or vaccinations, aiding in strategic planning and decision-making.

This solution ensures that the Medical Research Team can securely manage and analyze global health data, providing each country’s Health Minister with the insights they need to make informed decisions regarding public health and disease control efforts.

**Skills******

**Cloud Computing**: Used Google Cloud Storage (GCS) and BigQuery for secure, scalable data storage and processing.

**Data Engineering**: Developed an ELT pipeline with Apache Airflow for automating data extraction, transformation, and loading.

**Security**: Implemented row-level security and role-based access control (RBAC) using Google Cloud IAM to restrict access to country-specific data.

**Data Visualization**: Created interactive Looker dashboards and reports for Health Ministers to analyze disease data.

**SQL & Data Transformation**: Used SQL in BigQuery to query and transform data efficiently.

**Automation**: Automated data workflows and scheduling using Apache Airflow DAGs for streamlined processing.

**Conclusion**

This project provides an end-to-end solution for building an efficient ELT data pipeline on GCP, with automation and orchestration via Apache Airflow
