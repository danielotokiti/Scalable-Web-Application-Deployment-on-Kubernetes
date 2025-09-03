# Day 2 - Kubernetes Monitoring with Prometheus & Grafana
## Tasks Completed:
- Installed the kube-prometheus-stack Helm chart, which bundles Prometheus, Grafana, Alertmanager, node-exporter, and kube-state-metrics.
- Verified Prometheus was scraping Pod, Node, and Cluster metrics automatically (no app endpoint required).
- Configured port-forwarding to Grafana (kubectl port-forward svc/prometheus-grafana 3000:80 -n monitoring) to access dashboards locally.
- Explored cluster-wide dashboards for CPU, Memory, Pod restarts, and Node traffic.
- Confirmed observability of the Currency API pods as part of the monitored workloads.


## Screenshots:
- Helm installation logs (showing kube-prometheus-stack being deployed).
- kubectl get pods -n monitoring → shows Prometheus + Grafana pods running.
- Grafana login page (via port-forward).
- Grafana dashboard – Node CPU/Memory usage (prove cluster-level metrics).
- Grafana dashboard – Pod resource usage for Currency API (filtered by namespace = default).
- Prometheus Targets page .
