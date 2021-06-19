FROM openjdk:8
LABEL name="Venkat"
LABEL Env="Practice"
ENV applicationpath='/springpetclinic.jar'
ENV workingdirectory='/spc'
ENV dummy_tst="tst_dummy"
ARG dl_loc="https://referenceappkhaja.s3-us-west-2.amazonaws.com/spring-petclinic-2.2.0.BUILD-SNAPSHOT.jar"
RUN mkdir ${workingdirectory}
WORKDIR ${workingdirectory}
ADD ${dl_loc} ${workingdirectory}/${applicationpath}
EXPOSE 8080
CMD [ "java", "-jar", ${workingdirectory}/${applicationpath}  ]