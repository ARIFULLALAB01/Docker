FROM amazoncorretto:17-alpine3.17-jdk
LABEL author="khaja" 
LABEL project="learning"
EXPOSE 8080
# creates a new group and user
RUN addgroup -g 1000 spc && adduser -h "/spc" -u 1000 -G spc -s /bin/bash -D spc
# switching to user spc
USER spc
# Download the file
ADD --chown=spc:spc https://referenceapplicationskhaja.s3.us-west-2.amazonaws.com/spring-petclinic-3.1.0-SNAPSHOT.jar /spc/spring-petclinic-3.1.0-SNAPSHOT.jar
WORKDIR /spc
CMD ["java", "-jar", "spring-petclinic-3.1.0-SNAPSHOT.jar"]



#eXCERCISES --2
#FROM amazoncorretto:17-alpine3.17-jdk
#LABEL author="khaja" 
#LABEL project="learning"
#ADD https://referenceapplicationskhaja.s3.us-west-2.amazonaws.com/spring-petclinic-3.1.0-SNAPSHOT.jar /spc/spring-petclinic-3.1.0-SNAPSHOT.jar
#WORKDIR /spc
#EXPOSE 8080
#CMD ["java", "-jar", "spring-petclinic-3.1.0-SNAPSHOT.jar"]

#EXCERCISES--1
#FROM amazoncorretto:17-alpine3.17-jdk
#LABEL author="khaja" 
#LABEL project="learning"
#RUN wget https://referenceapplicationskhaja.s3.us-west-2.amazonaws.com/spring-petclinic-3.1.0-SNAPSHOT.jar
#EXPOSE 8080
#CMD ["java", "-jar", "spring-petclinic-3.1.0-SNAPSHOT.jar"]