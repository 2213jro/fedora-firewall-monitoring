# Project Overview

## Introduction

The Fedora Firewall Monitoring Project was created to gain hands-on experience with Linux administration, infrastructure monitoring, and technical documentation.

The project combines Fedora Linux, Prometheus, Grafana, and Node Exporter to create a monitoring environment capable of collecting, storing, and visualizing system performance metrics.

Rather than simply deploying software, the goal was to understand how each component interacts and to develop practical troubleshooting and validation skills that can be applied in real-world IT environments.

## Project Objectives

The primary objectives of this project were:

* Deploy a Fedora Linux server
* Implement a monitoring stack using Prometheus and Grafana
* Collect and visualize system metrics
* Practice Linux administration and service management
* Validate monitoring functionality through testing
* Create professional technical documentation

## Skills Demonstrated

This project demonstrates experience with:

### Linux Administration

* Fedora Linux deployment and configuration
* Package management
* Service management using systemd
* Basic network administration

### Monitoring and Observability

* Prometheus configuration
* Node Exporter deployment
* Grafana dashboard creation
* Infrastructure monitoring concepts

### Troubleshooting

* Service validation
* Monitoring verification
* Dependency analysis
* Log review and problem resolution

### Documentation

* Project documentation
* Architecture documentation
* Installation procedures
* Lessons learned and project analysis

## Monitoring Validation

A key component of this project involved validating the monitoring environment.

To confirm that monitoring was functioning correctly, the Node Exporter service was intentionally stopped. Grafana successfully detected the interruption and displayed missing metrics. Once the service was restarted, monitoring resumed normally.

This exercise demonstrated the importance of testing monitoring systems rather than assuming they are operating correctly.

## Project Value

This project provided practical experience with technologies commonly used in Linux and infrastructure environments.

In addition to technical skills, it reinforced the importance of documentation, validation, and troubleshooting when building and maintaining production systems.

## Future Development

Planned enhancements include:

* Firewall-specific monitoring
* Security-focused dashboards
* Alerting and notifications
* Multi-host monitoring
* Centralized logging
* Additional infrastructure metrics

## Conclusion

The Fedora Firewall Monitoring Project served as both a learning experience and a portfolio project. It provided hands-on exposure to Linux administration, monitoring technologies, troubleshooting methodologies, and technical documentation while creating a foundation for future infrastructure and cybersecurity projects.
