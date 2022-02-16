# Rundeck / Prometheus / Grafana integration demo via Rundeck Exporter

This is a demo environment that shows how to monitor a [Rundeck](https://github.com/rundeck/rundeck/) instance using [Rundeck Exporter](https://github.com/phsmith/rundeck_exporter) (thanks to @phsmith!), [Prometheus](https://github.com/prometheus/prometheus), and [Grafana](https://github.com/grafana/grafana) with [this](https://github.com/phsmith/rundeck_exporter/blob/main/examples/grafana/Rundeck-Dashboard.json) dashboard.

## Prerequisites

1. Docker.
2. Docker-compose.
3. A decent modern web browser :-)

## Getting the source

`git clone https://github.com/rundeck/rundeck-exporter-demo`

## Building the environment

  1. Go to the cloned repository directory.
  2. Build the environment with `docker-compose build`.

## Running the environment

  1. Just do `docker-compose up`.

## Testing the environment

  1. Open the `http://localhost:3000` URL in your web browser (user `admin`, password `admin`) and then select the "Rundeck" dashboard.
  2. Open a new tab with the `http://localhost:4440` URL (user `admin`, password `admin`) and create a new project with a job, do some executions.
  3. If you check the first browser tab (you will see all Rundeck instance metrics updated on the Grafana dashboard).

## Screenshot

<img width="1387" alt="Screen Shot 2021-11-12 at 12 12 34" src="https://user-images.githubusercontent.com/51376003/141489354-98412265-2609-4ac1-b91f-316de2d7ed8a.png">

