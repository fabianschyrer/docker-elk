ARG ELK_VERSION

# https://github.com/elastic/elasticsearch-docker
# FROM docker.elastic.co/elasticsearch/elasticsearch-oss:${ELK_VERSION}
# FROM docker.elastic.co/elasticsearch/elasticsearch:5.5.3
# FROM docker.elastic.co/elasticsearch/elasticsearch:6.4.2
FROM docker.elastic.co/elasticsearch/elasticsearch:latest

# Add your elasticsearch plugins setup here
# Example: RUN elasticsearch-plugin install analysis-icu
RUN elasticsearch-plugin install repository-s3
# RUN elasticsearch-plugin install x-pack
RUN elasticsearch-plugin install ingest-attachment
# RUN elasticsearch-plugin install ingest-user-agent
RUN elasticsearch-plugin install discovery-file
RUN elasticsearch-plugin install discovery-ec2
RUN elasticsearch-plugin install analysis-icu
