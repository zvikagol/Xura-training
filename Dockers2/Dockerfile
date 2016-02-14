FROM centos:latest
MAINTAINER zvikagol

ENV NAME xxx
RUN yum -y install java-1.8.0-openjdk-devel.x86_64
RUN yum -y install tomcat.noarch
RUN /bin/bash -c 'mkdir -p /logs'
ADD ./spring-petclinic-zviallan-1.0.0-20160214.123223-1.war /usr/share/tomcat/webapps/petclinic.war
CMD /usr/sbin/tomcat start && tail -f /logs/catalina.out
