FROM docker.elastic.co/logstash/logstash:7.17.25

# Install the azure_blob_storage plugin
#RUN bin/logstash-plugin install logstash-input-azure_blob_storage --version 0.12.10
RUN bin/logstash-plugin install logstash-input-azure_blob_storage
COPY conf.d/logstash.conf /usr/share/logstash/pipeline/logstash.conf
COPY conf.d/jvm.options /usr/share/logstash/config/jvm.options
