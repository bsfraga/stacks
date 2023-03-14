# grafana + prometheus

In this example, we are running Grafana, Prometheus, and Node Exporter as separate services within a Docker network called "monitoring". Grafana is exposed on port `3000`, Prometheus on port `9090`, and Node Exporter on port `9100`.

We are also mounting volumes for Grafana data and Prometheus data to persist their configurations. Additionally, we have added a provisioning folder in the volumes section to allow for the addition of your own configuration files for Grafana.

To integrate your Docker containers with Prometheus, you can add a `prometheus.yml` file to the `./prometheus` folder, which will define the targets to scrape.