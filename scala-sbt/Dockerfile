FROM log0ymxm/java
MAINTAINER paulnglsh@gmail.com

RUN echo 'deb https://dl.bintray.com/sbt/debian /' > /etc/apt/sources.list.d/sbt.list &&\
    apt-get update && \
    apt-get install -y --force-yes sbt=0.13.13 && \
    apt-get clean autoremove -y && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

RUN sbt