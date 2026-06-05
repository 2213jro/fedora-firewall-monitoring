# Screenshots

This folder contains screenshots documenting the deployment, monitoring, validation, and recovery testing performed during the Fedora Firewall Monitoring Project.

## Dashboard Overview

The primary Grafana dashboard displaying key infrastructure metrics.

![Grafana Dashboard](grafana-dashboard-overview.png)

---

## Service Health Monitoring

Node Exporter operating normally and successfully reporting metrics to Prometheus.

![Node Exporter Status](node-exporter-status.png)

---

## CPU Monitoring

CPU utilization monitored through Node Exporter and visualized in Grafana.

![CPU Monitoring](cpu-monitoring.png)

---

## Memory Monitoring

Real-time memory utilization monitoring.

![Memory Monitoring](memory-monitoring.png)

---

## Disk Monitoring

Disk usage monitoring for capacity and storage management.

![Disk Monitoring](disk-monitoring.png)

---

## Network In Monitoring

Inbound network traffic collected from monitored interfaces.

![Network In Monitoring](network-in-monitoring.png)

---

## Network Out Monitoring

Outbound network traffic visualization.

![Network Out Monitoring](network-out-monitoring.png)

---

## System Load Monitoring

System load monitoring used to identify resource utilization trends.

![System Load Monitoring](system-load-monitoring.png)

---

## System Uptime Monitoring

Server uptime monitoring demonstrating system availability and stability.

![System Uptime Monitoring](uptime-monitoring.png)

---

## Monitoring Validation Test

To validate the monitoring environment, the Node Exporter service was intentionally stopped.

Grafana successfully detected the outage and displayed the service as unavailable.

![Node Exporter Outage Test](node-exporter-outage-test.png)

---

## Service Recovery Validation

After restarting the Node Exporter service, Grafana resumed metric collection and reported the service as operational.

This confirmed that the monitoring stack could successfully detect both service failures and recoveries.

![Node Exporter Recovery Test](node-exporter-recovery-test.png)
