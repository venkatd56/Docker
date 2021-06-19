FROM ubuntu:18.04
RUN apt update && apt install openjdk-8-jdk wget -y && apt install curl -y
ENV applpath="/spc"
ARG dl_loc="https://referenceappkhaja.s3-us-west-2.amazonaws.com/spring-petclinic-2.2.0.BUILD-SNAPSHOT.jar"
RUN mkdir ${applpath}
ADD ${dl_loc} ${applpath}"/springpetclinic.jar"
EXPOSE 8080
CMD ["java", "-jar", ${applpath}"/springpetclinic.jar"]
HEALTHCHECK --interval=1m --timeout=2s --retries=3 CMD curl -f http://localhost/ || exit 1