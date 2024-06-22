ARG METRICBEAT_VERSION

FROM docker.elastic.co/beats/metricbeat:$METRICBEAT_VERSION
COPY --chown=root:metricbeat metricbeat.docker.yml /usr/share/metricbeat/metricbeat.yml