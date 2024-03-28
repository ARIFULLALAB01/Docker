FROM amazoncorretto:17-alpine3.17-jdk
LABEL author="Arifulla" 
LABEL project="SPCDummyProject"
ADD https://spcjarfile.blob.core.windows.net/spcjarfile/spring-petclinic-3.1.0-SNAPSHOT.jar /spc/spring-petclinic-3.1.0-SNAPSHOT.jar
WORKDIR /spc
EXPOSE 8080
CMD ["java", "-jar", "spring-petclinic-3.1.0-SNAPSHOT.jar"]