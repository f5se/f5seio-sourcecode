---
title: "Visualize your F5 and Apps"
date: 2022-11-280T8:41:13+08:00
draft: false
hideLastModified: true
summaryImage: "f5visual.jpg"
keepImageRatio: yes
tags: ["f5", "visualization", "grafana", "Partner"]
summary: "Quickly simulate API request to F5 control plane"
showInMenu: false
---



This is a brand new visualization powered by **Hu** Yipeng (胡易鹏) .

By combining Prometheus+Elasticsearch+Grafana to build a large screen for displaying F5 device status and business operation status.

- Prometheus combined with snmp-exporter is used to monitor the running status of equipment
- Elasticsearch combined with F5 HSL to display business operation status
- Grafana is used for large-screen view display

In word under this directory, you can see complete and detailed installation and configuration steps. related display

| **Dashboard template name**                | **Grafana data source** | **Function**                                            |
| ------------------------------------------ | ----------------------- | ------------------------------------------------------- |
| F5 equipment status monitoring             | Prometheus              | Monitor F5 device hardware status                       |
| Container&Node performance monitoring      | Prometheus              | Monitor the host hardware status                        |
| HTTP business view display                 | Elasticsearch-http      | Show F5 HTTP business status                            |
| Display of DNS resolution view             | Elasticsearch-dns       | Demonstrate F5 DNS service status                       |
| TCP-L4 delay view display                  | Elasticsearch-tcp       | Demonstrate the status of F5 L4 business chain building |
| Security protection situation view display | Elasticsearch-asm       | Show F5 Awaf security protection posture                |

Visual display effect of DNS resolution:

[![image-20221129164756426](img/image-20221129164756426.png)](https://github.com/myf5/f5-elk-demo/blob/master/NEW-Prometheus-elasticsearch-grafana/img/image-20221129164756426.png)

HTTP access visualization effect:

[![image-20221129164811794](img/image-20221129164811794.png)](https://github.com/myf5/f5-elk-demo/blob/master/NEW-Prometheus-elasticsearch-grafana/img/image-20221129164811794.png)

TCP connection delay display effect:

[![image-20221129164821310](img/image-20221129164821310.png)](https://github.com/myf5/f5-elk-demo/blob/master/NEW-Prometheus-elasticsearch-grafana/img/image-20221129164821310.png)

Display effect of security protection situation:

[![image-20221129164843441](img/image-20221129164843441.png)](https://github.com/myf5/f5-elk-demo/blob/master/NEW-Prometheus-elasticsearch-grafana/img/image-20221129164843441.png)

Host indicator monitoring display effect:

[![image-20221129164904264](img/image-20221129164904264.png)](https://github.com/myf5/f5-elk-demo/blob/master/NEW-Prometheus-elasticsearch-grafana/img/image-20221129164904264.png)

Display effect of container monitoring indicators:

[![image-20221129165023587](img/image-20221129165023587.png)](https://github.com/myf5/f5-elk-demo/blob/master/NEW-Prometheus-elasticsearch-grafana/img/image-20221129165023587.png)
