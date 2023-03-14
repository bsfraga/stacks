# Scraper

### Observations
Note that `host.docker.internal` is the hostname of the Docker host machine from within the container network. The `9323` port is the default port for Prometheus to scrape metrics from Docker.

After running `docker-compose up -d`, you should be able to access Grafana at `http://localhost:3000` and log in with the default credentials `(admin/admin)`. From there, you can add a Prometheus data source and create your own dashboards to visualize the metrics and logs from your Docker containers.

