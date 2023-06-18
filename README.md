Deploy Docker Compose Prometheus (with basic auth) + Grafana monitoring

## Files
- docker-compose.yml - docker compose file
- prometheus.yml - Prometheus configuration
- generate_web_yml.sh - web.yml generator (https://github.com/bgelov/prometheus-web-yml)

## Generating web.yml
```
chmod u+x generate_web_yml.sh
./webyml-generator.sh
```
and after moving web.yml to prometheus directory:
```
 mv web.yml prometheus/
```


## Run docker compose
```
docker compose up -d
```
