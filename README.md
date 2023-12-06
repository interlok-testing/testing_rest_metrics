# Interlok Rest Metrics, Prometheus and Grafana Testing

[![license](https://img.shields.io/github/license/interlok-testing/testing_rest_metrics.svg)](https://github.com/interlok-testing/testing_rest_metrics/blob/develop/LICENSE)
[![Actions Status](https://github.com/interlok-testing/testing_rest_metrics/actions/workflows/gradle-build.yml/badge.svg)](https://github.com/interlok-testing/testing_rest_metrics/actions/workflows/gradle-build.yml)

## What it does

This project show how we can use Interlok rest metrics with Prometheus and Grafana.

There are two channels with two workflows each.

The first channel has two HTTP enpoints, one for a successful scenario and one for a failing scenario.

The second channels is querying the success HTTP endpoint every 5 seconds and the fail HTTP endpoint every 30 seconds.


## Getting started

```shell
./gradlew clean install

docker-compose up -d
```

## Dashboards:

- JVM: http://localhost:3000/d/K9kmttsGk/jvm
- Interlok: http://localhost:3000/d/XyHj4tsMk/interlok

## Prometheus:

- workflow_avgnanos: http://localhost:9090/graph?g0.expr=workflow_avgnanos&g0.tab=1&g0.stacked=0&g0.range_input=1h
- workflow_count_total: http://localhost:9090/graph?g0.expr=workflow_count_total&g0.tab=1&g0.stacked=0&g0.range_input=1h
