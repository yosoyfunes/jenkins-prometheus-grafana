# Jenkins Prometheus Grafana
Monitoring Jenkins with Prometheus and Grafana

The repository will install for you Jenkins with plugins pre-instaled, Prometheus, Grafana

Start with Git Clone
```
git clone https://github.com/yosoyfunes/jenkins-prometheus-grafana

docker-compose build --pull --no-cache
docker-compose up --detach
```

## Visit the web UI by browsing to:

```bash
Jenkins    http://localhost:8080/
Prometheus http://localhost:9090/
Grafana    http://localhost:3000/

"For Login Use: admin:admin"
```

## Grafana Dashboard:
- Jenkins: Performance and Health Overview (ID: 9964)
- Node Exporter for Prometheus Dashboard (ID: 1860)
- Node Exporter Full (ID: 11074)

## If you want to login into Docker container:
```bash
docker-compose exec <prometheus/grafana/jenkins> bash
```

## When you're done, you can shut down the cluster using:

```bash
docker-compose down
```