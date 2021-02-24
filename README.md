# Interlok, Prometheus and Grafana

```shell
gradle clean install
docker-compouse up -d
```

Dashboards:

- [JVM](http://localhost:3000/d/K9kmttsGk/jvm)
- [Interlok](http://localhost:3000/d/XyHj4tsMk/interlok)

Prometheus:

- [workflow_avgmillis](http://localhost:9090/graph?g0.expr=workflow_avgmillis&g0.tab=1&g0.stacked=0&g0.range_input=1h)
