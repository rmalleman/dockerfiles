FROM rmalleman/java
MAINTAINER malleman@rmalleman@gmail.com

RUN echo 'deb https://dl.bintray.com/sbt/debian /' > /etc/apt/sources.list.d/sbt.list &&\
    apt-get update && \
    apt-get install -y --force-yes sbt=0.13.13 && \
    apt-get install -y --force-yes mysql-client && \
    apt-get install -y --force-yes docker.io && \
    apt-get clean autoremove -y && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* && \
    pip install awscli

RUN sbt
