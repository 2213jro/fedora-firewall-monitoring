# Installation Guide

## Objective

Deploy a Fedora Linux server and implement a monitoring stack using Prometheus, Grafana, and Node Exporter.

## Fedora Linux Installation

### Initial Setup

- Installed Fedora Linux Server
- Configured network settings
- Created administrative user account
- Updated system packages

```bash
sudo dnf update -y
```

## Node Exporter Installation

### Download Node Exporter

```bash
wget https://github.com/prometheus/node_exporter/releases/latest/download/node_exporter-*.linux-amd64.tar.gz
```

### Configure Service

- Created Node Exporter service account
- Created systemd service
- Enabled service at boot

## Prometheus Installation

### Install Prometheus

- Downloaded Prometheus binaries
- Created configuration file
- Configured scrape targets
- Enabled Prometheus service

## Grafana Installation

### Install Grafana Repository

- Added Grafana repository
- Installed Grafana Server
- Started and enabled service

## Validation

Verified access to:

- Grafana Web Interface
- Prometheus Targets Page
- Node Exporter Metrics Endpoint

## Outcome

Successfully deployed a complete monitoring stack capable of collecting and visualizing infrastructure metrics.
