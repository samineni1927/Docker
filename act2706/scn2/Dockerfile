FROM openjdk:11
LABEL author "Sharath"
EXPOSE 8080
RUN adduser -D appuser && mkdir /home/appuser/sample
USER appuser
WORKDIR /home/appuser/sample
ADD --chown=appuser https://referenceapplicationskhaja.s3.us-west-2.amazonaws.com/spring-petclinic-2.4.2.jar /home/appuser/sample/spring-petclinic-2.4.2.jar
CMD ["java", "-jar", "/home/appuser/sample/spring-petclinic-2.4.2.jar"]