# Secure Grafana Access Configuration

## Overview

After deploying Prometheus, Grafana, and Node Exporter, the monitoring platform was initially accessible only through the local Grafana web interface on port 3000.

To improve usability and provide secure remote access, Grafana was configured behind a reverse proxy and published through a dedicated subdomain:

**watchtower.pschi02.com**

This configuration provides a professional monitoring endpoint that can be accessed securely through HTTPS.

---

## Objectives

* Eliminate the need to access Grafana through port 3000
* Provide a memorable monitoring URL
* Enable encrypted HTTPS connections
* Improve accessibility for future project expansion
* Create a production-style monitoring environment

---

## Technologies Used

* Fedora Linux
* Grafana
* Nginx Reverse Proxy
* DNS Configuration
* SSL/TLS Certificates
* DigitalOcean Cloud Infrastructure

---

## Implementation Process

### 1. DNS Configuration

A dedicated subdomain was created:

watchtower.pschi02.com

The DNS record was configured to point to the Fedora monitoring server.

### 2. Reverse Proxy Configuration

Nginx was configured as a reverse proxy to forward incoming web traffic to the Grafana service running locally on port 3000.

Traffic Flow:

User Browser
↓
watchtower.pschi02.com
↓
Nginx Reverse Proxy
↓
Grafana (localhost:3000)

### 3. HTTPS Configuration

SSL/TLS certificates were installed and configured to secure communications between users and the monitoring platform.

Benefits include:

* Encrypted traffic
* Improved security
* Browser trust validation
* Professional deployment standards

### 4. Validation Testing

The monitoring platform was tested to verify:

* DNS resolution
* HTTPS functionality
* Dashboard accessibility
* Metric collection
* Service availability

All tests completed successfully.

---

## Results

The Grafana monitoring platform is now accessible through:

https://watchtower.pschi02.com

The deployment provides secure, centralized access to infrastructure monitoring dashboards without requiring direct access to Grafana's default port.

---

## Lessons Learned

This phase of the project provided hands-on experience with:

* DNS management
* Reverse proxy configuration
* SSL/TLS certificate deployment
* Secure web application publishing
* Infrastructure monitoring architecture

The implementation transformed the monitoring environment from a locally accessible service into a professionally published monitoring platform.
