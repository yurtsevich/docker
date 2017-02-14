FROM yurtsevich/jre
MAINTAINER Dzmitry Yurtsevich (d.yurtsevich@gmail.com)

ENV WILDFLY_VERSION 10.1.0.Final
ENV INSTALL_DIR /opt

RUN cd ${INSTALL_DIR} && curl http://download.jboss.org/wildfly/${WILDFLY_VERSION}/wildfly-${WILDFLY_VERSION}.tar.gz | tar zx

# To add a user for management console
# RUN $JBOSS_HOME/bin/add-user.sh admin admin --silent

ENV DEPLOYMENT_DIR ${INSTALL_DIR}/wildfly-${WILDFLY_VERSION}/standalone/deployments/

EXPOSE 8080 9990
CMD ["/opt/wildfly-10.1.0.Final/bin/standalone.sh", "-b", "0.0.0.0"]
