## Description
MKTXP is a Prometheus Exporter for Mikrotik RouterOS devices.

This is **Kubernetes** fork from original version [mktxp](https://github.com/akpw/mktxp)

## Install:
1. Edit [kubernetes/mikrotik-exporter.yml](https://github.com/koss822/mktxp/blob/main/kubernetes/mikrotik-exporter.yml)
2. Install
```
kubectl apply -f mikrotik-exporter.yml
```