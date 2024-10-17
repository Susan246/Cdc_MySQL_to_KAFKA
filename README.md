# Cdc_MySQL_to_KAFKA
- This repository contains implementations of both single-node and multi-node setups for Apache Kafka, managed by Zookeeper. The project demonstrates the use of Python for data streaming and processing. Please refer the document I have attached there you can have the youtube links to setup enviroments as well as links of other documents.

## Overview
The project includes:

A single-node Kafka and zookeeper 
A three-node Kafka cluster utilizing Zookeeper.
Python program for data processing and interaction with Kafka.
Also airbyte is used for same task and I have attached the docker-compose file.

## Architecture
The architecture consists of:

Zookeeper: Manages Kafka brokers and maintains metadata.
Python Scripts: Scripts that facilitate data processing and interaction with Kafka. Using python for cdc of mysql and pass to kafka topics
Kafka:  Kafka captures and streams real-time changes from the database to other applications.

## Usage
To run the single-node Kafka setup, execute the appropriate Python program
For the multi-node Kafka setup, navigate to the relevant directory and follow the instructions provide in documents
