# KubernetesMonitoring using Prometheus and Grafana



Prometheus Architecture

![image](https://github.com/KarthiCholan/KubernetesMonitoring/assets/108706606/2a637cbe-d8c0-4247-8b96-77119c28f372)



What is Prometheus?

Prometheus is an open source monitoring tool
Provides out-of-the-box monitoring capabilities for the Kubernetes container orchestration platform. It can monitor servers and databases as well.
Collects and stores metrics as time-series data, recording information with a timestamp 
It is based on pull and collects metrics from targets by scraping metrics HTTP endpoints.

What is Grafana?

Grafana is an open source visualization and analytics software. 
It allows you to query, visualize, alert on, and explore your metrics no matter where they are stored.

Why System monitoring is critical?

Alerting: can give early warning of issues or problems before they become serious, costly or irreversible.

Visibility: Monitoring provides real-time insights into the health and performance of your applications and infrastructure.

Capacity Planning: By collecting and analyzing data over time, you can make informed decisions about capacity planning, such as when to add or remove nodes, allocate more resources, or scale your applications.






#  Prequisities

AWS EKS Cluster

HELM Should be installed
