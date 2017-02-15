FROM yurtsevich/wildfly
MAINTAINER Dzmitry Yurtsevich (d.yurtsevich@gmail.com)

COPY newrelic-java-3.35.2.zip ${JBOSS_HOME}

RUN cd ${JBOSS_HOME} \
    && unzip newrelic-java-3.35.2.zip \
    && rm newrelic-java-3.35.2.zip \
    && cd newrelic \
    && java -jar newrelic.jar install
