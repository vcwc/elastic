ARG  VCW_TAG=5.0.18
FROM vcwc/bash.rest:${VCW_TAG}

COPY ./_image /vcw/
RUN chmod -R +x /vcw/bin

ENV VWC_REALM=vcwc \
    VWC_LIBRARY=elastic \
    VWC_IMAGE=search \
    VWC_FLAVOR=rest \
    VWC_TAG=${VCW_TAG} \
    VWC_IMAGENAME=vcwc/elastic.search.rest

LABEL co.vcweb.schema-version="1.0" \
      co.vcweb.label="vcwc/elastic.search.rest Image" \
      co.vcweb.description="Bash base REST client for ElasticSearch." \
      co.vcweb.realm="vcwc" \
      co.vcweb.library="elastic" \
      co.vcweb.image="search" \
      co.vcweb.flavor="rest" \
      co.vcweb.tag="${VCW_TAG}" \
      co.vcweb.maintainer="vcw@vcweb.co"
