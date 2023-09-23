# library

In this chart, my helm charts will be stored and can be used in a kubernetes cluster.

```bash
cd [DIRECTORY_WITH_HELM_CHART]
helm package [CHARTNAME] -d [CHART_REPO_DIRECTORY]

cd [CHART_REPO_DIRECTORY]
helm repo index charts
```

Check, that the repository has been published as github pages.

Commit the chart into this github project and use it in kubernetes

```bash
helm repo add mkoellges https://mkoellges.github.io/library/charts

helm install pgo mkoellges/pgo
```
