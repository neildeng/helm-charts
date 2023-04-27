# LGTM-Stack Helm Chart

## Prerequisites

Make sure you have Helm [installed](https://helm.sh/docs/using_helm/#installing-helm).


## Deploy Loki、Grafana、Tempo and Mimir to your cluster, include Kube-Prometheus-stack and Phlare

### Deploy with default config

```bash
helm upgrade --install lgtm grafana/lgtm-stack
```

### Deploy in a custom namespace

```bash
helm upgrade --install lgtm --namespace=lgtm-stack grafana/lgtm-stack
```

### Deploy with custom config

```bash
helm upgrade --install lgtm grafana/lgtm-stack --set "key1=val1,key2=val2,..."
```
