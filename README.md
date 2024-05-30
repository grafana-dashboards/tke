# grafana-dashboards-tke

Grafana Dashboards for TKE(Tencent Kubernetes Engine).

## Grafana installation recommendations

`values` for [grafana chart](https://github.com/grafana/helm-charts/blob/main/charts/grafana/README.md):

```yaml
sidecar:
  dashboards:
    folderAnnotation: "grafana_folder"
    provider:
      foldersFromFilesStructure: true
```

## Usage

```bash
git clone --depth 1 git@github.com:grafana-dashboards/tke.git grafana-dashboards-tke
kubectl apply -k ./grafana-dashboards-tke
```
