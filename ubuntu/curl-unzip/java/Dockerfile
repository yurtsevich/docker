FROM yurtsevich/curl-unzip
MAINTAINER Dzmitry Yurtsevich (d.yurtsevich@gmail.com)
RUN apt-get update \
    && apt-get install -y openjdk-8-jre
ENV JAVA_HOME /usr/lib/jvm/java-8-openjdk-amd64
ENV PATH "$PATH":$JAVA_HOME/bin
CMD ["bash"]