## HELM Demo:

## Create HELM Chart: 
```
helm create <chart_name>
helm create todo-api
```
This will create a directory structure with all files and folder.
```
chars/
templates/                  # this folder has all k8 manifest files    
  _helpers.tpl
  deployment.yaml
  hpa.yaml
  ingress.yamk
  NOTES.txt
  service.yaml
  serviceaccount.yaml
  .helmignore
chart.yaml                  # Contains chart details like chartname, chartversion, appversion
values.yaml                 # this has all variables details in JINJA template
```

