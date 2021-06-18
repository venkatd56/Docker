# Base Image from Centos
FROM centos:7
#Generate Labels
LABEL author="venkatd"
LABEL EMAIL="venkat.tet@gmail.com"
LABEL Org="Airforce"
# update Packages and install httpd
RUN yum update -y && yum install httpd -y
ENTRYPOINT ["echo"]
CMD ["hello-world"]
