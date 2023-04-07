
## Kubernetes version

![License](https://img.shields.io/badge/License-GNU%20GPL-blue.svg)
![Language](https://img.shields.io/badge/python-v3.6-blue)
![License](https://img.shields.io/badge/mikrotik-routeros-orange)
![License](https://img.shields.io/badge/prometheus-exporter-blueviolet)


## Description
MKTXP is a Prometheus Exporter for Mikrotik RouterOS devices.\
It gathers and exports a rich set of metrics across multiple routers, all easily configurable via built-in CLI interface. 

While simple to use, MKTXP supports [advanced features](https://github.com/akpw/mktxp#advanced-features) such as automatic IP address resolution with both local & remote DHCP servers, concurrent exports across multiple router devices, configurable data processing & transformations, etc.

Apart from exporting to Prometheus, MKTXP can print selected metrics directly on the command line (see examples below). 

For effortless visualization of the RouterOS metrics exported to Prometheus, MKTXP comes with a dedicated [Grafana dashboard](https://grafana.com/grafana/dashboards/13679):

<img width="32%" alt="1" src="https://user-images.githubusercontent.com/5028474/217029083-3c2f561e-853f-45a7-b9f1-d818a830daf5.png"> <img width="32%" alt="2" src="https://user-images.githubusercontent.com/5028474/217029092-2b86b41b-1f89-4383-ac48-16652e820f7e.png"> <img width="32%" alt="3" src="https://user-images.githubusercontent.com/5028474/217029096-dbf6b46c-3ed7-4c76-a57b-8cebfb3b671c.png">


#### Requirements:
- Supported OSs:
   * Linux   
   * Mac OSX
   * FreeBSD

- Mikrotik RouterOS device(s)

- Optional: 
   * [Prometheus](https://prometheus.io/docs/prometheus/latest/installation/)
   * [Grafana](https://grafana.com/docs/grafana/latest/installation/)
   * [Docker](https://docs.docker.com/) / [Docker Compose](https://docs.docker.com/compose/)


## Install:
There are multiple ways to install this project, from a standalone app to a [fully dockerized monitoring stack](https://github.com/akpw/mktxp-stack). The supported options include:
- [MKTXP Stack](https://github.com/akpw/mktxp-stack): a ready-to-go MKTXP monitoring stack

- from [Docker image](https://github.com/akpw/mktxp/pkgs/container/mktxp) : `❯ docker pull ghcr.io/akpw/mktxp:latest`

- from [PyPI](https://pypi.org/project/mktxp/): `❯ pip install mktxp`

- latest from source repository: `❯ pip install git+https://github.com/akpw/mktxp`




## Getting started
To get started with MKTXP, you need to edit its main configuration file. This essentially involves filling in your Mikrotik devices IP addresses & authentication info, optionally modifying various settings to specific needs. 

The default configuration file comes with a sample configuration, making it easy to copy / edit parameters for your RouterOS devices as needed and is saved in **kubernetes/** directory