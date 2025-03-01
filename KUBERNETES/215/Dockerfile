FROM centos

MAINTAINER apasoft.training@gmail.com

RUN mkdir /opt/tomcat/

WORKDIR /opt/tomcat
RUN curl -O https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.100/bin/apache-tomcat-9.0.100.tar.gz
RUN tar xvfz apache*.tar.gz
RUN mv apache-tomcat-9.0.100/* /opt/tomcat/.
RUN curl -O https://download.java.net/java/GA/jdk18.0.1.1/65ae32619e2f40f3a9af3af1851d6e19/2/GPL/openjdk-18.0.1.1_linux-x64_bin.tar.gz
RUN tar xvfz openjdk*.tar.gz

WORKDIR /opt/tomcat/webapps
COPY app1.war .
EXPOSE 8080