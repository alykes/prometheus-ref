# Quick reference for Prometheus 

References: https://prometheus.io/docs/introduction/overview/


## Node Exporter (Linux)
source location: https://github.com/prometheus/node_exporter

### Example installation
```wget https://github.com/prometheus/node_exporter/releases/download/v1.0.0/node_exporter-1.0.0.linux-amd64.tar.gz```

```tar xvfz node_exporter-1.0.0.linux-amd64.tar.gz```

```cd node_exporter-1.0.0.linux-amd64/```

 - Run the exporter manually

```./node_exporter```

## Node Exporter (Windows)
source location: https://github.com/prometheus-community/windows_exporter/releases

```
iwr -useb -o windows_exporter-0.16.0-amd64.exe https://github.com/prometheus-community/windows_exporter/releases/download/v0.16.0/windows_exporter-0.16.0-amd64.exe
```

- Run the exporter manually

```.\windows_exporter-0.16.0-amd64.exe```

   or to only collect certain metrics

```.\windows_exporter-0.16.0-amd64.exe --collectors.enabled "os,cpu,logical_disk"```
