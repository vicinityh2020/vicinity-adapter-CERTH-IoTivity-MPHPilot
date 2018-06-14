# 1. Infrastructure overview
This is a Vicinity Adapter for MPH Pilot infrastructure.It is used to describe motion sensors, door sensors, pressure mats and panic buttons, which are deployed in municipality houses and is based on IoTivity Platform.

# 2. Configuration and deployment
## Requirements

JDK 1.8
Apache Maven 3.3.9 or higher

## Build using Maven

In the root folder of the project:

`mvn clean install`

## Run
In the target folder of the project:

`java -jar adapter-0.0.1-SNAPSHOT.jar`

# 3. Functionality and API

## Endpoints
*	GET /objects (optional): Retrieve all devices Thing Descriptions(TDs) for registration to VICINITY. This functionality is optional since auto-registration of devices will be performed.

## Functions
*	Send device TDs to the vicinity agent at start up
*	Publish every new measurement to a specific Vicinity event topic
