ARG LOGSTASH_INDEXER_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/logstash/logstash:${LOGSTASH_INDEXER_VERSION}

# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json
RUN logstash-plugin install logstash-integration-kafka
