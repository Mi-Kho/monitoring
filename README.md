# monitoring
Monitoring Linux systems
## Table of contents
- [Prometheus](#prometheus)
- [Grfana](#grafana)
- [cAdvisor](#cadvisor)
- [Node Exporter](#node-exporter)

This [file](https://github.com/Mi-Kho/monitoring/blob/main/docker-compose.yml) will run docker compose for Prometheus, Grafana and cAdvisor.

## Prometheus

Configuration file is in /etc/prometheus/[prometheus.yml](https://github.com/Mi-Kho/monitoring/blob/main/prometheus/prometheus.yml)

## Grafana

Add new Connection for Prometheus in Home > Connections > Data sources > Prometheus :

http://prometheus:9090

## cAdvisor

Use this [repo](https://github.com/google/cadvisor).

## Node exporter

for Node Exporter run this :

~~~
wget https://github.com/prometheus/node_exporter/releases/download/v*/node_exporter-*.*-amd64.tar.gz #replace version
tar xvfz node_exporter-*.*-amd64.tar.gz #replace version
cd node_exporter-*.*-amd64 #replace version
./node_exporter
~~~

You can also use this [repo](https://github.com/prometheus/node_exporter).

## DCGM Exporter

Docker hub:
nvidia/dcgm-exporter:3.2.5-3.1.7-rc1-ubuntu20.04


