# Fedora Firewall Monitoring Project

## Overview

This project documents the deployment and monitoring of a Fedora Linux firewall using Prometheus, Grafana, and Node Exporter. The goal was to gain hands-on experience with Linux administration, infrastructure monitoring, troubleshooting, and observability while building a portfolio-ready project.

As part of the project, monitoring functionality was validated by intentionally stopping services and confirming that outages were detected and reported through Grafana dashboards.

## Project Goals

- Deploy and configure a Fedora Linux firewall
- Implement infrastructure monitoring using Prometheus and Grafana
- Collect and visualize system performance metrics
- Validate monitoring through service outage testing
- Develop documentation and troubleshooting procedures

## Technologies Used

- Fedora Linux
- Prometheus
- Grafana
- Node Exporter
- systemd
- Linux Networking

## Architecture

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
Grafana Dashboard
```

## Features

- CPU Monitoring
- Memory Monitoring
- Disk Usage Monitoring
- Network Traffic Monitoring
- System Load Monitoring
- Uptime Monitoring
- Service Health Validation

## Screenshots

Screenshots will be added as the project progresses.

## Validation Testing

To verify monitoring functionality, the Node Exporter service was intentionally stopped. Grafana successfully detected the outage and displayed the service interruption. After restarting the service, monitoring metrics resumed normally.

This test confirmed that the monitoring stack was functioning correctly and capable of detecting service failures.

## Lessons Learned

- Linux service management using systemd
- Infrastructure monitoring fundamentals
- Prometheus metric collection
- Grafana dashboard creation
- Monitoring validation and troubleshooting
- Documentation best practices

## Future Improvements

- Firewall-specific metrics
- Security event monitoring
- Alertmanager integration
- Email notifications
- Multi-host monitoring
- Log aggregation and analysis

## Author

Jose Rojas

Per Scholas IT Support Student
