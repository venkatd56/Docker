#Base image
FROM openjdk:8
#Labels
LABEL name="Venkat"
LABEL email="venkat.tt@t.com"
LABEL env="dev"
#Set Variables
ENV applpath='/springpetclinic.jar'
ARG dl_loc="https://referenceappkhaja.s3-us-west-2.amazonaws.com/spring-petclinic-2.2.0.BUILD-SNAPSHOT.jar"
ADD ${dl_loc} ${appl_path}
EXPOSE 8080
CMD ["java",  "-jar",  ${applpath}} ] 
