FROM centos:centos7

ADD apache-tomcat-8.5.66.tar.gz /usr/local/

ENV MYPATH /usr/local
WORKDIR $MYPATH

RUN yum install -y java-1.8.0-openjdk

EXPOSE 8080
EXPOSE 80

CMD /usr/local/apache-tomcat-8.5.66/bin/startup.sh && tailf /usr/local/apache-tomcat-8.5.66/logs/catalina.out
