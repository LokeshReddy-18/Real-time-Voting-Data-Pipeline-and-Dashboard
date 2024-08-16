# Real-time-Voting-Data-Pipeline-and-Dashboard
This project sets up a comprehensive real-time voting data pipeline using Apache Kafka and Apache Spark, and provides a dynamic dashboard for monitoring and analyzing election results.

## Overview
The system comprises two main components:

Real-time Data Pipeline: Processes and aggregates voting data in real-time.
Dashboard: Provides real-time updates and visualizations for election statistics.

## Real-time Data Pipeline
Components
Apache Kafka: Used for message streaming and data ingestion.

Topics:
* votes_topic: Receives raw voting data from various sources.
* aggregated_votes_per_candidate: Stores aggregated vote counts per candidate.
* aggregated_turnout_by_location: Stores voter turnout data by location.


## Apache Spark: Handles real-time data processing and aggregation.

* Data Processing:
Schema Definition: Defines the structure of the incoming voting data.
* Data Ingestion: Reads data from the Kafka votes_topic.
Preprocessing: Includes data type casting and watermarking for handling late data.
* Aggregation:
Votes per Candidate: Aggregates total votes by candidate.
Turnout by Location: Aggregates voter turnout by geographical location.
.

## Workflow

Data Ingestion: Voting data is streamed from various sources into Kafka.
Processing: Spark reads from Kafka, applies schema, and preprocesses the data.
Aggregation: Spark performs real-time aggregations to summarize vote counts and turnout.
Output: Aggregated results are pushed to Kafka topics for further consumption or visualization.

## Dashboard
Components
Streamlit: Framework for creating an interactive web-based dashboard.
Kafka Python Client: For consuming real-time data from Kafka.
Pandas: For data manipulation and analysis.
Matplotlib: For visualizations such as bar charts, pie charts, and donut charts.
Features

## Reference
Realtime Voting System | End-to-End Data Engineering Project : https://www.youtube.com/watch?v=X-JnC9daQxE&t=2393s


## Conclusion
This project provides a robust real-time data pipeline and interactive dashboard for monitoring and analyzing election data. It leverages the power of Kafka and Spark for data processing and Streamlit for delivering an engaging user experience.

