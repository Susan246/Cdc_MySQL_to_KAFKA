# Cdc_MySQL_to_KAFKA
This repository contains implementations of both single-node and multi-node setups for Apache Kafka, managed by Zookeeper, and also  with integration with Airbyte for data ingestion. The project demonstrates the use of Python for data streaming and processing.

Overview
The project includes:

A single-node Kafka and zookeeper 
A three-node Kafka cluster utilizing Zookeeper.
Integration with Airbyte for easy data ingestion from various sources.
Python scripts for data processing and interaction with Kafka.
Architecture
The architecture consists of:

Zookeeper: Manages Kafka brokers and maintains metadata.
Kafka: The messaging system for high-throughput data streaming.
Airbyte: A tool for integrating data from different sources into Kafka.
Python Scripts: Scripts that facilitate data processing.
Requirements
Kafka: Version 2.x or higher
Zookeeper: Version 3.x or higher
Python: Version 3.7 or higher
Airbyte: Version 0.x
Docker (optional): For setting up Kafka and Zookeeper
Installation
To set up the project, please follow these steps:

1. Prerequisites
Before setting up and running the Kafka streaming job, ensure that the following requirements are met:

i. Software Requirements:
MySQL: Version 5.7 or higher (version 8 is recommended), with binlog enabled. The binlog format should be mixed-based to capture schema-level changes (e.g., add, delete, modify columns); otherwise, row-based can capture row-level changes. MySQL Downloads

Kafka/Confluent-Kafka: Version 2.5 or higher (latest version recommended), properly configured and running. Kafka Downloads | Confluent Installation Guide

Zookeeper: Required by Kafka for coordination (no need to download separately as it comes bundled with Kafka).

Java: JDK 1.8 or higher installed (Java 11 is recommended). Java Downloads

Python: Python 3 is recommended. Install the following libraries to connect with MySQL and Kafka:

confluent_kafka
pymysqlreplication
pymysql
You can install these libraries using:

bash
Copy code
pip install PyMySQL
pip install pymysqlreplication
pip install confluent-kafka
Python Downloads

Docker (optional): For running Kafka, Zookeeper, MySQL, and Airbyte in containers.

ii. Permissions and Access:
MySQL User: A MySQL user with the necessary permissions for reading binlog data. Ensure the user has the following privileges:
REPLICATION SLAVE
REPLICATION CLIENT
SELECT
2. Set Up Kafka and Zookeeper:
Follow the instructions in the 3_node_kafka_and_3_node_zookeeper directory for a multi-node setup.
For single-node instructions, check the single_node_kafka_and_zookeeper directory.
3. Install Required Python Packages:
Navigate to the project directory and install the necessary Python packages using your preferred package manager.
4. Set Up Airbyte:
Refer to the airbyte directory for installation and configuration details.
Usage
To run the single-node Kafka setup, execute the appropriate Python script.
For the multi-node Kafka setup, navigate to the relevant directory and follow the instructions provided in the README files within.
