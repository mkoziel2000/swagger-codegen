FROM openjdk:8-windowsservercore

WORKDIR /generator

COPY target/lib/jetty-runner* /generator/jetty-runner.jar
COPY target/*.war /generator/swagger-generator.war

ENV GENERATOR_HOST=192.168.6.247

EXPOSE 8080

CMD ["java", "-jar", "/generator/jetty-runner.jar", "/generator/swagger-generator.war"]

