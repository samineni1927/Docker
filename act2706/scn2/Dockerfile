FROM openjdk:11
LABEL author "Sharath"
EXPOSE 8080
RUN useradd -m appuser 
USER appuser
WORKDIR /home/appuser
ADD --chown=appuser https://referenceapplicationskhaja.s3.us-west-2.amazonaws.com/spring-petclinic-2.4.2.jar /home/appuser/spring-petclinic-2.4.2.jar
CMD ["java", "-jar", "/home/appuser/spring-petclinic-2.4.2.jar"]