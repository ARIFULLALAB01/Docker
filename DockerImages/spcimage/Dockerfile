FROM amazoncorretto:17-alpine3.17-jdk
LABEL author="Arifulla"
LABEL project="learning"
ADD https://spcjarfile.blob.core.windows.net/spcjar/spring-petclinic-3.2.0-SNAPSHOT.jar /spring-petclinic-3.1.0-SNAPSHOT.jar
EXPOSE 8080
CMD ["java", "-jar", "spring-petclinic-3.1.0-SNAPSHOT.jar"]