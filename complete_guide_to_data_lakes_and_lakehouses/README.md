# [Complete Guide to Data Lakes and Lakehouses](https://www.linkedin.com/learning/complete-guide-to-data-lakes-and-lakehouses)

* Provider: LinkedIn Learning
* Author: Thalia Barrera

## Technologies

* MinIO: S3-compatible storage layer
* Apache Iceberg: table format
* Dremio: query engine
* DBT: data transformation
* Dagster: Data Orchestration
* Apache Superset: analytics and visualization
* LangChain and Chroma: Advanced Gererative AI applications

## Architecture

We will be using the "Medallion Architecture":

1. Bronze
2. Silver
3. Gold

## Data Lake

### Definition

A Data Lake is a centralized repository designed to store a vast amount of structured and unstructured data. It allows for the storage of data at any scale and in its native format, which can be used for various types of analytics such as real-time analytics, machine learning, and artificial intelligence.

### Key Characteristics

* Scalability: Data Lakes can efficiently handle and store vast amounts of data—up to petabytes and beyond—without significant performance issues.
* Cost-effectiveness: Leveraging object storage, Data Lakes provide a more affordable solution for storing large data volumes, compared to traditional storage methods.
* Flexibility: Data can be stored in various formats including logs, XML, JSON, images, and more, sourced from diverse origins.
* Accessibility: Centralized data storage in Data Lakes facilitates easier access for data scientists and analysts, enhancing their ability to derive insights quickly using integrated tools.

### Use Cases

* Data science and machine learning: Serve as foundational platforms for handling diverse data formats essential for developing sophisticated models
* Artificial intelligence: Enable the training of more effective AI models by managing large sets of varied data
* Real-time analytics: Support immediate data processing needs, helping businesses swiftly respond to market dynamics
* Evolution of Data Lakes

## Hadoop

### Definition

From the digital data explosion in the late 1990s and early 2000s, the advent of big data brought challenges that traditional data systems couldn't handle, leading to the development of Hadoop and subsequently the concept of data lakes. This evolution was closely tied to advancements in cloud computing, which further facilitated the adoption of data lakes by providing scalable, secure, and cost-effective storage solutions.

### Key Characteristics

* Inspired by Google MapReduce and Google File System.
* Designed to store and process huge amounts of data across distributed clusters.
* Democratized raw data storage.
* Conceptual beginning of the data lake.
* Closely tied to the advancement of cloud computing.
* AWS, Azure, and GC became robust and the perfect ecosystem for data lakes.
* Cloud platforms offered scalable, secure, and cost effective storage.

### Data Democratization

* This is another key factor in the rise of data lakes.
* By centralizing data storage, data lakes enable a collaborative environment.

## Architecture Core Components

* Storage Layer: The foundation that holds massive amounts of raw data in various formats, designed to be scalable, cost-effective, and support multiple data types.
* Ingestion Layer: Responsible for reliably collecting data from diverse sources in real-time or batches, handling high volumes and speeds.
* Processing Layer: Transforms and aggregates data, applying business rules to prepare data for analysis, supporting both batch and real-time processing.
* Management and Governance Layer: Ensures data security, organization, metadata management, and compliance with regulations.
* Analytics Layer: Provides tools for querying, visualizing, and analyzing data efficiently, making data actionable for users.

## Data Warehouse

A data warehouse is a system designed for reporting and data analysis, serving as a core part of business intelligence. It stores current and historical data in a single place, organizing it in a highly structured way using tables, rows, and columns with a defined schema. This structure enables fast and complex SQL queries, making it ideal for generating reports and supporting decision-making. Unlike data lakes, data warehouses require data to be cleaned and transformed before or after storage to ensure quality and consistency.

### Data Lake vs Data Warehouses

* Data Structure: Data warehouses store highly structured data using predefined schemas (tables, rows, columns), enabling fast SQL queries. Data lakes store raw data without predefined schemas, applying structure only when data is read.
* Data Processing: Data warehouses require data to be cleaned and transformed before or after storage to ensure quality and consistency. Data lakes ingest raw data quickly with minimal upfront processing, offering flexibility but needing more processing power during analysis.
* Storage Technology and Cost: Data warehouses use optimized relational database systems, while data lakes often rely on scalable, cost-effective technologies like Hadoop or cloud object storage (e.g., Amazon S3).
* Use Cases: Data warehouses are ideal for business intelligence, reporting, and decision-making. Data lakes are better suited for exploratory data analysis, machine learning, and AI applications.

## Data Mesh

### Definition

A data mesh is a modern data architecture approach that treats data as a product. Instead of centralizing data governance and management in one team, it decentralizes ownership to domain-specific teams who manage their own data. This ensures the data is accessible, high-quality, and valuable across the organization. Unlike a centralized data lake, data mesh promotes a decentralized architecture where different teams may use different storage or processing systems based on their needs. This approach is especially useful for large, distributed organizations with complex data across multiple business domains, enabling agile and autonomous data management by specialized teams.

### Data Lake vs Data Mesh

* Governance: Data lakes are centrally governed by data engineering teams managing access, security, and quality. Data mesh decentralizes governance, with domain-specific teams owning and managing their data as a product.
* Architecture: Data lakes are centralized repositories storing vast amounts of raw and structured data in one place. Data mesh promotes a decentralized architecture where different teams may use different storage or processing systems based on their needs.
* Use Cases: Data lakes suit organizations needing centralized data storage for analytics. Data mesh fits large, distributed organizations with complex data domains, enabling agile, autonomous data management by specialized teams.

## [Storage in Data Lakes](storage_in_data_lakes.md)