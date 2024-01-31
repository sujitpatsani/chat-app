# Read Me First
The following was discovered as part of building this project:

* The original package name 'com.hld.chat-app' is invalid and this project uses 'com.hld.chatapp' instead.

# Getting Started

#KAFKA

Step-1 
Install Docker desktop 

Step-2 
Run docker compose file
command -docker compose -f docker-compose.yml up -d

Step-3
Move into Kafka container
docker exec -it <kafka_conatiner_id> /bin/sh
Go inside kafka installation folder
cd /opt/kafka_<version>/bin

Step-4
Create Kafka topic
kafka-topics.sh --create --zookeeper zookeeper:2181 --replication-factor 1 --partitions 1 --topic quickstart

### Reference Documentation
For further reference, please consider the following sections:

* [Official Apache Maven documentation](https://maven.apache.org/guides/index.html)
* [Spring Boot Maven Plugin Reference Guide](https://docs.spring.io/spring-boot/docs/3.2.2/maven-plugin/reference/html/)
* [Create an OCI image](https://docs.spring.io/spring-boot/docs/3.2.2/maven-plugin/reference/html/#build-image)
* [Spring Web](https://docs.spring.io/spring-boot/docs/3.2.2/reference/htmlsingle/index.html#web)
* [WebSocket](https://docs.spring.io/spring-boot/docs/3.2.2/reference/htmlsingle/index.html#messaging.websockets)

### Guides
The following guides illustrate how to use some features concretely:

* [Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)
* [Serving Web Content with Spring MVC](https://spring.io/guides/gs/serving-web-content/)
* [Building REST services with Spring](https://spring.io/guides/tutorials/rest/)
* [Using WebSocket to build an interactive web application](https://spring.io/guides/gs/messaging-stomp-websocket/)

