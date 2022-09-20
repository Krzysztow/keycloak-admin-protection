FROM jboss/keycloak:15.0.2

COPY ./docker-build /wd

RUN /opt/jboss/keycloak/bin/jboss-cli.sh --file=/wd/admin-realm-https-port-change.cli
RUN /opt/jboss/keycloak/bin/jboss-cli.sh --file=/wd/block-keycloak-welcome.cli
