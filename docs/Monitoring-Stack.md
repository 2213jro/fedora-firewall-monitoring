# Monitoring Stack

## Purpose

The monitoring stack provides visibility into the health and performance of the Fedora Linux firewall.

## Components

### Grafana

Visualization platform used to create dashboards and monitor system health.

### Prometheus

Time-series database responsible for collecting and storing metrics.

### Node Exporter

Exports operating system metrics to Prometheus.

## Metrics Collected

### CPU

- CPU utilization
- CPU load

### Memory

- Memory utilization
- Available memory

### Storage

- Disk utilization
- Disk capacity

### Network

- Network traffic
- Transmit and receive statistics

### System

- Uptime
- Service availability

## Dashboard Features

- Real-time monitoring
- Historical performance analysis
- Infrastructure visibility
- Service health validation

## Outage Testing

To validate monitoring functionality:

1. Node Exporter service was stopped.
2. Metrics stopped reporting.
3. Grafana displayed service interruption.
4. Node Exporter was restarted.
5. Metrics resumed successfully.

This confirmed the monitoring environment was functioning as expected.
