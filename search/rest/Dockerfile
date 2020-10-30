ARG  VCW_TAG=7.9.2
ARG  VCW_TAG_BASH=5.0.18
FROM vcwc/bash.rest:${VCW_TAG_BASH}

COPY ./_image /vcw/
RUN chmod -R +x /vcw/bin

ENV VCW_REALM=vcwc \
    VCW_LIBRARY=elastic \
    VCW_IMAGE=search \
    VCW_FLAVOR=rest \
    VCW_TAG=${VCW_TAG} \
    VCW_IMAGENAME=vcwc/elastic.search.rest

LABEL co.vcweb.schema-version="1.0" \
      co.vcweb.label="vcwc/elastic.search.rest Image" \
      co.vcweb.description="Bash base REST client for ElasticSearch." \
      co.vcweb.realm="vcwc" \
      co.vcweb.library="elastic" \
      co.vcweb.image="search" \
      co.vcweb.flavor="rest" \
      co.vcweb.tag="${VCW_TAG}" \
      co.vcweb.maintainer="vcw@vcweb.co"
