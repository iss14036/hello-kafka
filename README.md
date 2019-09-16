# Go Event Source

## Problem Statement
Simple project of how to impelement kafka with java as producer and consumer. If you don't know what kafka is, you can refer to [here](https://kafka.apache.org/quickstart)

## How it works
A streaming platform has three key capabilities:

- Publish and subscribe to streams of records, similar to a message queue or enterprise messaging system.
- Store streams of records in a fault-tolerant durable way.
- Process streams of records as they occur.

Kafka is generally used for two broad classes of applications:

- Building real-time streaming data pipelines that reliably get data between systems or applications
- Building real-time streaming applications that transform or react to the streams of data

To understand how Kafka does these things, let's dive in and explore Kafka's capabilities from the bottom up.
First a few concepts:

- Kafka is run as a cluster on one or more servers that can span multiple datacenters.
- The Kafka cluster stores streams of records in categories called topics.
- Each record consists of a key, a value, and a timestamp.
![Github Logo](https://kafka.apache.org/23/images/kafka-apis.png)

For further information, you can open [here](https://kafka.apache.org/intro)

## Dependencies
In this time, I use mac as an os to running the system.

#### 1. Java

## How to use
To run kafka, first you have to run zookeeper, by this following command :
```$xslt
bin/zookeeper-server-start.sh config/zookeeper.properties
```
And after that, you can start the kafka
```$xslt
bin/kafka-server-start.sh config/server.properties
```

You can run the program by running this command at terminal :
```
./gradlew run producer/Sender
```
