# Real-time Data transportation and Ingestion

### Introduction

Welcome to a three part tutorial series on real-time data ingesting and analysis.  The speed of today's processing systems have moved from classical data warehousing batch reporting to the realm of real-time processing and analytics. The result is real-time business intelligence. Real-time means near to zero latency and access to information whenever it is required. This tutorial will show how geolocation information from trucks can be combined with sensor data from trucks and roads.  These sensors report real-time events like speeding, lane-departure, unsafe tailgating, and unsafe following distances. We will capture these events in real-time.

## Pre-Requisites

*  Downloaded and Installed latest [Hortonworks Sandbox](http://hortonworks.com/products/hortonworks-sandbox/#install)
*  [Learning the Ropes of the Hortonworks Sandbox](http://hortonworks.com/hadoop-tutorial/learning-the-ropes-of-the-hortonworks-sandbox/)
*   8GB+ RAM (Assigning more is recommended) and preferably 4 processor cores, otherwise you may encounter errors in the third tutorial
*   Data sets used:
  *   New York City Truck Routes from NYC DOT.
  *   Truck Events Data generated using a custom simulator.
  *   Weather Data, collected using APIs from Forcast.io.
  *   Traffic Data, collected using APIs from MapQuest.

All data sets used in these tutorials are real data sets but modified to fit these use cases

## Tutorial Overview

The events generated by sensors will be captured through a distributed publish-subscribe messaging system named Apache Kafka. We will use Apache Storm to process this data from Kafka and eventually persist that data into HDFS and Hbase.

## Goals of the tutorial

*   Understanding real-time data analysis.
*   Understanding Apache Kafka architecture.
*   Creating Producers and Consumers in Kafka.
*   Understanding Apache Storm architecture.
*   Creating Spouts and Bolts in Storm.
*   Persisting data from Storm into Hive and Hbase

## Outline

1.  Tutorial Introduction
2.  Pre-Requisites:
  -  Data sets used:
  -  Downloaded and Installed latest [Hortonworks Sandbox](http://hortonworks.com/products/hortonworks-sandbox/#install)
  -  [Learning the Ropes of the Hortonworks Sandbox](http://hortonworks.com/hadoop-tutorial/learning-the-ropes-of-the-hortonworks-sandbox/)
3.  Tutorial Overview
4.  Goals of the Tutorial
5.  Concepts:
  -  [Apache Kafka](rtep-concepts.md)
  -  [Apache Storm](rtep-concepts.md)
  -  [Apache Kafka on Storm](rtep-concepts.md)
6.  Get Started with HDP labs:
  - Lab 1: [Apache Kafka: Real-time event stream transportation](rtep-1.md)
  - Lab 2: [Apache Storm: Processing real-time event stream](rtep-2.md)
  - Lab 3: [Hive & Hbase: Persisting real-time event stream](rtep-3.md)
7.  Next Steps/Try these
8.  References