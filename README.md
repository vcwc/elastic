# `vcwc/elastic` Image Library

The repository of stacks and modules build from the official ElasticSearch images.

These are all the ElasticSearch images that follow the ElasticSearch version.

## APM Server

### vcwc/elastic/apm_server

The APM Server base stack and module.

## ElasticSearch Beats

### vcwc/elastic/filebeat

A new entrypoint is added to the official image so the nodename and custom configuration can be picked up automatically.

### vcwc/elastic/filebeat/file

Filebeat stack and module pre-configured for file input.

### vcwc/elastic/filebeat/file/sasl

Filebeat stack and module pre-configured for file input and SASL authenticated output.

### vcwc/elastic/filebeat/kafka

Filebeat stack and module pre-configured for kafka input.

### vcwc/elastic/filebeat/kafka/sasl

Filebeat stack and module pre-configured for kafka input and SASL authenticated output.

### vcwc/elastic/heartbeat

A new entrypoint is added to the official image so the nodename and custom configuration can be picked up automatically.

Implements base Heartbeat stack and module.

### vcwc/elastic/journalbeat

A new entrypoint is added to the official image so the nodename and custom configuration can be picked up automatically.

Implements base Journalbeat stack and module.

### vcwc/elastic/journalbeat/sasl

Implements Journalbeat stack and module pre-configured for SASL authenticated output.

### vcwc/elastic/metricbeat

A new entrypoint is added to the official image so the nodename and custom configuration can be picked up automatically.

Implements base MetricBeat stack and module.

### vcwc/elastic/metricbeat/node

Implements MetricBeat stack and module pre-configured for host metrics.

### vcwc/elastic/metricbeat/overlay

Implements MetricBeat stack and module pre-configured for service metrics.

## Kibana

### vcwc/elastic/kibana

Implements a Kibana base stack and module, port mounted and served at root.

### vcwc/elastic/kibana/traefik

Implements a standard url mounted Kibana stack and module configured for Traefik reverse proxy.

## ElasticSearch

### vcwc/elastic/search

The ElasticSearch base stack.

### vcwc/elastic/search/rest

Basic REST client for ElasticSearch.

### vcwc/elastic/search/traefik

Implements a standard url mounted ElasticSearch stack and module configured for Traefik reverse proxy.

## ElasticSearch Based Stacks

### vcwc/elastic/stacks/eka

The ElasticSearch - Kibana - APM Server base stack and module.

### vcwc/elastic/stacks/eka/traefik

The ElasticSearch - Kibana - APM Server base stack and module configured for Traefik reverse proxy.

### vcwc/elastic/stacks/ekg

The ElasticSearch - Kibana - Grafana base stack and module.

### vcwc/elastic/stacks/eka/traefik

The ElasticSearch - Kibana - Grafana base stack and module configured for Traefik reverse proxy.
