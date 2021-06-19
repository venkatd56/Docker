FROM ubuntu:18.04
RUN apt update && apt install openjdk-8-jdk wget -y
ENV applpath='/springpetclinic.jar'
ARG dl_loc="https://referenceappkhaja.s3-us-west-2.amazonaws.com/spring-petclinic-2.2.0.BUILD-SNAPSHOT.jar"
RUN mkdir ${applpath}
ADD ${dl_loc} ${appl_path}
EXPOSE 8080
CMD ["java",  "-jar",  ${applpath} ] 
