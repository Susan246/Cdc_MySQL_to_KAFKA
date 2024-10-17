# Cdc_MySQL_to_KAFKA
- This repository contains implementations of both single-node and multi-node setups for Apache Kafka, managed by Zookeeper, and also  with integration with Airbyte for data ingestion. The project demonstrates the use of Python for data streaming and processing. Please refer the document I have attached there you can have the youtube links to setup enviroments as well as links of other documents.

## Overview
The project includes:

A single-node Kafka and zookeeper 
A three-node Kafka cluster utilizing Zookeeper.
Integration with Airbyte for easy data ingestion from various sources.
Python scripts for data processing and interaction with Kafka.

## Architecture
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

## Usage
To run the single-node Kafka setup, execute the appropriate Python script
For the multi-node Kafka setup, navigate to the relevant directory and follow the instructions provide in documents
