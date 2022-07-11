FROM maven:3-openjdk-11 AS builder
RUN git clone https://github.com/spring-projects/spring-petclinic.git && cd spring-petclinic && mvn package

FROM openjdk:11
LABEL author=Sharath
COPY --from=builder /spring-petclinic/target/spring-petclinic-2.7.0-SNAPSHOT.jar /spring-petclinic-2.7.0-SNAPSHOT.jar
EXPOSE 8082
CMD ["java", "-jar", "/spring-petclinic-2.7.0-SNAPSHOT.jar"]