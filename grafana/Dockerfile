ARG GRAFANA_IMAGE
FROM ${GRAFANA_IMAGE}

COPY data/datasources.yml /etc/grafana/provisioning/datasources/
COPY data/rundeck.yml /etc/grafana/provisioning/dashboards/
COPY data/rundeck.json /var/lib/grafana/dashboards/