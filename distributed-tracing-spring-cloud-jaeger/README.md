# Distributed tracing with Spring cloud Jaeger

In this project I have figured out how we can integrate distributed tracing using spring cloud jaeger which is based on Opentracing. 

Once you build the application using `mvn clean verify`, You can start the application as two service instances. 

Service 1
```
java -jar \
target/Distributed-Service-0.0.1-SNAPSHOT.jar \
--spring.application.name=Service-1 \
--server.port=8080
```

Service 2
```
java -jar \
target/Distributed-Service-0.0.1-SNAPSHOT.jar \
--spring.application.name=Service-2 \
--server.port=8090
```
