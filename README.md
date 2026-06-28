# k8s observability stack

Helm chart for Prometheus + Grafana + Alertmanager. Similar to what I ran on EKS before just installing kube-prometheus-stack everywhere.

```
charts/k8s-observability-stack/
```

Node exporter dashboard baked in via ConfigMap. Alerts go to email through Alertmanager — you'll want to swap in your SMTP settings in values.yaml.

```sh
helm install observability ./charts/k8s-observability-stack
```
