# Architecture

## Overview

The Fedora Firewall Monitoring Project consists of a Fedora Linux server monitored through Prometheus and visualized using Grafana dashboards.

## Components

### Fedora Linux Firewall

The primary server being monitored. Responsible for hosting firewall services and exporting system metrics.

### Node Exporter

Collects system-level metrics including:

- CPU utilization
- Memory usage
- Disk utilization
- Network activity
- System load
- Uptime

### Prometheus

Prometheus periodically scrapes metrics from Node Exporter and stores the data in a time-series database.

### Grafana

Grafana connects to Prometheus and provides dashboards for visualizing infrastructure health and performance.

## Data Flow

```text
Fedora Firewall
      │
      ▼
Node Exporter
      │
      ▼
Prometheus
      │
      ▼
Grafana
```

## Ports Used

| Service | Port |
|----------|--------|
| Node Exporter | 9100 |
| Prometheus | 9090 |
| Grafana | 3000 |

## Monitoring Workflow

1. Node Exporter collects system metrics.
2. Prometheus scrapes metrics at configured intervals.
3. Metrics are stored in Prometheus.
4. Grafana queries Prometheus.
5. Dashboards display system health and performance data.
