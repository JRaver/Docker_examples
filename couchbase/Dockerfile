FROM centos:centos6

MAINTAINER JRaver  <jraver@mail.ru>

RUN yum update  -y
RUN yum install -y pkgconfig 
RUN yum install -y http://packages.couchbase.com/releases/4.0.0/couchbase-server-community-4.0.0-centos6.x86_64.rpm
RUN echo "/opt/couchbase/bin/couchbase-server -- -noinput -detached > /opt/couchbase/var/lib/couchbase/logs/start.log 2>&1" > ~/.bashrc
EXPOSE 8091
