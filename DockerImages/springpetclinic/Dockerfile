FROM amazoncorretto:17-alpine3.17-jdk
LABEL author="Arifulla" 
LABEL project="SPCDummyProject"
EXPOSE 8080
# creates a new group and user
RUN addgroup -g 1000 spc && adduser -h "/spc" -u 1000 -G spc -s /bin/bash -D spc
# switching to user spc
USER spc
# Download the file
ADD https://spcjarfile.blob.core.windows.net/spcjarfile/spring-petclinic-3.1.0-SNAPSHOT.jar /spring-petclinic-3.1.0-SNAPSHOT.jar
WORKDIR /spc
CMD ["java", "-jar", "spring-petclinic-3.1.0-SNAPSHOT.jar"]

#ADD --chown=spc:spc https://spcjarfile.blob.core.windows.net/spcjarfile/spring-petclinic-3.1.0-SNAPSHOT.jar /spc/spring-petclinic-3.1.0-SNAPSHOT.jar