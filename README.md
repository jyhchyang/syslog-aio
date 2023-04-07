# syslog-aio
Review of Loki Syslog All-in-One stack

# References:
1. [Grafana - Loki - Syslog - AIO](https://grafana.com/grafana/dashboards/13766-loki-syslog-aio-overview/)
2. [Syslog-ng logging stack](https://www.syslog-ng.com/community/b/blog/posts/grafana-loki-syslog-ng-jump-starting-a-new-logging-stack)
3. [Github.com/lux4rd0](https://github.com/lux4rd0/grafana-loki-syslog-aio)


This Loki Syslog All-In-One example is geared to help you get up and running quickly with a Syslog ingestor and visualization of logs. 
It uses Grafana Loki and Promtail as a receiver for forwarded syslog-ng logs.

Essentially:

RFC3164 Network/Compute Devices -> syslog-ng (UDP port 514) -> Promtail (port 1514) -> Loki (port 3100) <- Grafana (port 3000)
