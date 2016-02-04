#Overview

This application provides the **Eureka Server** that provides service discivery and enables all Eureka clients to discover each other.

When a client registers with Eureka, it provides meta-data about itself such as host and port, health indicator URL, home page etc. Eureka receives heartbeat messages from each instance belonging to a service. If the heartbeat fails over a configurable timetable, the instance is normally removed from the registry.

##Pre-requisites

### Projects that need to be started before
* [config server](/../config-service/README.md) - For pulling the configuration information

### Running the application
* Build the application by running the `./gradlew clean build` gradle command at the "eureka-service" project root folder	on the terminal.
* If you want to run the application as jar file, then run `java -jar build/libs/eureka-service-0.0.1-SNAPSHOT.jar` command at the terminal.