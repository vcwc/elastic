ARG  VCW_TAG=7.9.2
FROM docker.elastic.co/beats/metricbeat:${VCW_TAG}

USER root
ENTRYPOINT ["/vcw/bin/docker-entrypoint"]
COPY ./_image/docker-entrypoint /vcw/bin/docker-entrypoint
RUN chmod -R 755 /vcw/bin/docker-entrypoint
#USER metricbeat

LABEL co.vcweb.schema-version="1.0" \
      co.vcweb.label="vcwc/elastic/metricbeat - External Build" \
      co.vcweb.description="The Official ElasticSearch Metricbeat image with amended entrypoint." \
      co.vcweb.realm="vcwc" \
      co.vcweb.library="elastic" \
      co.vcweb.image="metricbeat" \
      co.vcweb.flavor="" \
      co.vcweb.tag="${VCW_TAG}" \
      co.vcweb.maintainer="vcw@vcweb.co"
