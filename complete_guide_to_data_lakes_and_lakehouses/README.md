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

It is a centralized repository that allows you to store all of your structured and unstructured data at any scale.

### Key Characteristics

* Scalability
    * Can store petabytes of data
* Cost Effectiveness
    * Object storage costs less than traditional storage
* Flexibility
    * Can hold diverse data formats
* Accesibility
    * Centralized data storage

### When to use

* Data Science and Machine Learning
* Artifial Intelligence
* Real-Time Analytics

## Hadoop

### Definition

The data lake foundation.

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