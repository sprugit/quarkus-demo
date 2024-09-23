# quarkus-demo
Round up review demo project made to document the lessons learned over the course of my first year as a Java backend developer using Quarkus.

# What is Quarkus
Quarkus is a java framework, much in the vein of Spring, which allows us to build complex applications to the deployed over the web.
Quarkus follows a reactive programming style, with a single thread event-loop which processes I/O and delegates work to other [threads](https://quarkus.io/guides/virtual-threads).

# What is this project?
This project is an exercise in implementing a possible solution for an inventory tracking app for a small chain of grocery stores.
Each POS machine would have some sort of application which would produce a kafka-message whenever a sale occurs. This message would later be processed by a central set of consumers which would persist these changes to a database.
A third and final service will be a REST service which would allow an employee of our fake grocery store chain to access store inventory data.

# Scope of this project
The main focus of this project is the functional aspects and features of Quarkus, making use of reactive programming to develop this app. Therefore, database models along with any other miscellaneous potential improvements won't be further explored than necessary. My objective is to have a simple and clean barebones implementation of such an app.

# Technologies Used

- Maven
- Java Quarkus
- Apache Kafka
- Protobuf
- Docker-Engine
- Oracle SQL
- Git (obviously)
