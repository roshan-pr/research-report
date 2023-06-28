# Prometheus

Prometheus is an open-source technology designed to provide monitoring and alerting functionality for cloud-native environments, including Kubernetes. It can collect and store metrics as time-series data, recording information with a timestamp. It can also collect and record labels, which are optional key-value pairs.

### Key features of Prometheus include:

- **Multidimensional data model** – Using time-series data, which is identified by metric name and key-value pairs.

- **PromQL** – A flexible querying language that can leverage the multi-dimensional data model.

- **No reliance on distributed storage** – All single server nodes remain autonomous.

- **Pull model** – Prometheus can collect time-series data by actively “pulling” data over HTTP.

- **Pushing time-series data** – Available through the use of an intermediary gateway.

- **Monitoring target discovery** – Available through static configuration or service discovery.

- **Visualization** – Prometheus offers multiple types of graphs and dashboards.

## Working of Prometheus

To get metrics, Prometheus requires an exposed HTTP endpoint. Once an endpoint is available, Prometheus can start scraping numerical data, capture it as a time series, and store it in a local database suited to time-series data. Prometheus can also be integrated with remote storage repositories.

Users can leverage queries to create temporary times series from the source. These series are defined by metric names and labels. Queries are written in PromQL, a unique language that allows users to choose and aggregate time-series data in real time. PromQL can also help you establish alert conditions, resulting in notifications to external systems like email, PagerDuty, or Slack.

Prometheus can display collected data in tabular or graph form, shown in its web-based user interface. You can also use APIs to integrate with third-party visualization solutions like Grafana.

## Monitor with Prometheus

**Service Metrics :**
Prometheus is typically used to collect numeric metrics from services that run 24/7 and allow metric data to be accessed via HTTP endpoints. This can be done manually or with various client libraries. Prometheus exposes data using a simple format, with a new line for each metric, separated with line feed characters. The file is published on an HTTP server that Prometheus can query and scrape metrics from based on the specified path, port, and hostname.

Prometheus can also be used for distributed services, which are run on multiple hosts. Each instance publishes its own metrics and has a name that Prometheus can distinguish.

**Host Metrics :**
You can monitor the operating system to identify when a server’s hard disk is full or if a server operates constantly at 100% CPU. You can install a special exporter on the host to collect the operating system information and publish it to an HTTP-reachable location.

**Website Uptime/Up Status :**
Prometheus doesn’t usually monitor website status, but you can use a blackbox exporter to enable this. You specify the target URL to query an endpoint, and perform an uptime check to receive information such as the website’s response time. You define the hosts to be queried in the prometheus.yml configuration file, using relabel_configs to ensure Prometheus uses the blackbox exporter.

**Cronjobs :**
To check if a cronjob is running at the specified intervals, you can use the Push Gateway to display metrics to Prometheus through an HTTP endpoint. You can push the timestamp of the last successful job (i.e. a backup job) to the Gateway, and compare it with the current time in Prometheus. If the time exceeds the specified threshold, the monitor times out and triggers an alert.