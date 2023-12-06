# Interlok, Prometheus and Grafana

[![license](https://img.shields.io/github/license/interlok-testing/testing_rest_metrics.svg)](https://github.com/interlok-testing/testing_rest_metrics/blob/develop/LICENSE)
[![Actions Status](https://github.com/interlok-testing/testing_rest_metrics/actions/workflows/gradle-build.yml/badge.svg)](https://github.com/interlok-testing/testing_rest_metrics/actions/workflows/gradle-build.yml)

```shell
gradle clean install
docker-compose up -d
```

Dashboards:

- [JVM](http://localhost:3000/d/K9kmttsGk/jvm)
- [Interlok](http://localhost:3000/d/XyHj4tsMk/interlok)

Prometheus:

- [workflow_avgnanos](http://localhost:9090/graph?g0.expr=workflow_avgnanos&g0.tab=1&g0.stacked=0&g0.range_input=1h)
- [workflow_count_total](http://localhost:9090/graph?g0.expr=workflow_count_total&g0.tab=1&g0.stacked=0&g0.range_input=1h)
