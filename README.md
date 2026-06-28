# Kubernetes observability stack

Helm chart for a basic observability stack on K8s — Prometheus, Grafana, Alertmanager. Pattern I've used on a few EKS clusters.

## Components

- **Prometheus** — metrics collection
- **Grafana** — dashboards (Node Exporter overview pre-loaded via ConfigMap)
- **Alertmanager** — alert routing to email

## Chart layout

```
charts/k8s-observability-stack/
  Chart.yaml
  values.yaml
  templates/
    grafana-dashboard-configmap.yaml
```

## Deploy

```sh
helm install observability ./charts/k8s-observability-stack
```

```sh
helm uninstall observability
```

**Mamoon Idrees** · [LinkedIn](https://www.linkedin.com/in/mamoon-idrees) · mamoon.idrees5@gmail.com
