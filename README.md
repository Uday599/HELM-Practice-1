## HELM Demo:

## Create HELM Chart: 
```
helm create <chart_name>
helm create todo-api
```
### This will create a directory structure with all files and folder. 
```
todo-api/
chars/
templates/                  # this folder has all k8 manifest files    
  _helpers.tpl              # reusable helper template similar to function in python, which can be used anywhere, can be called using                                include
  deployment.yaml
  hpa.yaml
  ingress.yamk
  NOTES.txt                 # Plain text file created after template is deployed, contains information about what to do next after                                   helm installation
  service.yaml
  serviceaccount.yaml
  .helmignore
chart.yaml                  # Contains chart details like chartname, chartversion, appversion
values.yaml                 # this has all variables details in JINJA template
```

## Run lint before installaing the chart 

```
cd todo-api/
helm lint .
```

## Install chart
```
helm install <release_name> <path/to/helm/chart>
helm install todo-api .
```
