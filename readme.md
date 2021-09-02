# helm charts store to github page

## create git repository on github
...
## install helm cli
...

## create chart 
```bash
helm create test
```

## package chart 
```bash
helm package test/
helm repo index --url https://leson.github.io/helm-charts .
```

## push to git repository
```bash
git add . 
git commit -m "initial helm chart"
git push origin master
```

## setup githup pages on github

## add chart repo on local
```bash
helm repo add myrepo https://leson.github.io/helm-charts
helm repo list
helm search myrepo
```