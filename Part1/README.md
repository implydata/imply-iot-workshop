
# Real Time IoT Analytics - Introduction

In today’s world, there are about 17 billion IoT devices emitting data and is [projected](https://www.google.com/url?q=https://www.statista.com/statistics/1183457/iot-connected-devices-worldwide/&sa=D&source=editors&ust=1714417939339055&usg=AOvVaw0sxOzNNIKi3oFavKXcJPPk) to go up to 30 billion by 2030. New technologies have enabled such devices to be smaller than ever, more efficient, powerful and versatile.

Regardless, if businesses add these devices to old equipment or build new assets from scratch, the IoT brings cutting edge capabilities to such assets, such as connecting physical devices to the network helps end users  remotely monitor, analyze, control and automate their operations. Some of the common use cases that IoT transforms the way work is accomplished are:

*   Fleet Management of Electric Vehicles
*   Electric vehicle chargers

The more IoT enabled devices evolve, the need for analytics keeps growing. Some of the common industry challenges associated with IoT analytics, particularly in the context of real-time data processing are;

1.  ### Data Infrastructure for IoT:

*   *Challenge*: Designing robust data pipelines, storage solutions, and analytics stacks to handle the large volume of streaming data from IoT devices.

2.  ### Stream Processing:

*   *Challenge*: Real-time data streams from IoT devices require low latency processing. Traditional batch processing methods are inadequate.

3.  ### Data Integration Complexity:

*   *Challenge*: IoT devices often lack compatibility with each other. Integrating heterogeneous data streams is complex.

4.  ### Descriptive Analytics:

*   *Challenge*: Monitoring the status of IoT devices, identifying anomalies, and displaying current and historical sensor data.

5.  ### Diagnostic Analytics:

*   *Challenge*: Understanding why something is happening. Analyzing IoT data to identify core problems.

## Apache Druid to rescue

We at Imply have found solutions to some of the *Challenges* through Apache Druid, in the following manner,

*  **Anamoly Detection**, With Imply we have developed ability to enhance the dependability and safeguard the security of electric transportation networks, with a particular emphasis on the fleet management of electric vehicles (EVs). Utilizing extensive datasets, the research examines several facets of fault properties including, fault codes, motor temperature, charging stations, charging records, identified abnormalities, and other maintenance metrics. 

*   **Onboarding** multi-tenants of the above mentioned use cases is the primary pitfall. In the case of fleet management, each sensor from various assets such as electric vehicles emit data which can be varied. For instance, some vehicles emit motor\_temperatures while some others don’t, but may emit another metric on IGBT temperatures. Apache Druid has ways to include such telemetry changes, sometimes on the fly without having to make schema changes (schema auto-discovery).

*   **Scaling** these apps can pose a challenge in the long run with growing volume and complexity. When users want to view data at a granular level, to the most recent hour, in order to track assets such that business would not want assets to leave a particular radius, the app should be able to cater to the user. At the same time, when the leadership would like to view the monthly aggregated data for smart analysis on how the assets can be deployed in future, the same app should be able to provide that detail as well. Apache Druid has the ability to provide a granular view of customer data and rolled-up to attributes.



 ## Building Blocks for our Workshop today

![Architechture](https://github.com/implydata/imply-iot-workshop/blob/main/Part1/IoT%20Architectural%20building%20blocks.png "Architecture, Building Blocks")

*   **AWS IoT Data Simulator** (Simulates several virtual connected devices without having to configure and manage physical devices)
*   **AWS IoT Core** (Fully Managed MQTT message broker which helps build IoT architecture that are cost effective, relaible and optimized for scale)
*   **Kinesis** (Serverless streaminig data service to ingest audio, video, application logs, clisckstream, etc.)
*   **Imply Polaris** (Real time analytical database for fast query response and highly concurrent)


 
*Quick links :*
[Home](/README.md) - [Part 1](/Part1/README.md) - [Part 2](/Part2/README.md) - [Part 3](/Part3/README.md) - [Part 4](/Part4/README.md)
