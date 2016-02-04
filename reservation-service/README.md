#Overview

This application acts as a resource server and provides demo reservation related functionality and serves as one component. It defines the REST endpoints that are used to provide reservation functionality to client services.

Note that this component is only used internally by the "reservation" microservice and is NOT actually exposed at the API gateway level.

##Pre-requisites

### Projects that need to be started before
* [config service](/../config-service/README.md) - For pulling the configuration information
* [webserver-registry](/../eureka-service/README.md) - For starting the Eureka server since the authorization server also is a micro-service that needs to be registered with Eureka server.    

### Running the application
* Build the application by running the `./gradlew clean build` gradle command at the "registration-service" project root folder	on the terminal.
* If you want to run the application as jar file, then run `java -jar build/libs/registration-service-0.0.1-SNAPSHOT.jar` command at the terminal.