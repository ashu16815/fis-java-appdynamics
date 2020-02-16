FROM docker-registry-default.reg.ocp.internal.spark.co.nz/openshift/fuse-java-openshift:1.1

USER root

ADD appdynamics/ /opt/appdynamics/

RUN chgrp -R 0 /opt/appdynamics/
RUN chmod -R g+rw /opt/appdynamics/
RUN find /opt/appdynamics/ -type d -exec chmod g+x {} +

#jboss from FIS
USER 185
