# helm-charts
Fresh8 Custom helm charts

# Setup helm
```
helm init
```

# Creating a helm package
```
helm package ${DIR_PATH_TO_CHART_TO_ADD}
helm repo index . # Creates an index.yaml file that references this file - required for helm to use the repo
git add .
git commit -m "Add new Chart to fresh8 repo"
```

# Adding custom helm repo
```
helm repo add fresh8 'https://raw.githubusercontent.com/fresh8/helm-charts/master/'
helm repo update
helm search pachyderm
```
