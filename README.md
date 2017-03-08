# iron-ui-kubernetes
kuberntes deployment files for iron-ui
#Usage:
* Add your iron url to iron-ui-config.yaml:
```
kind: ConfigMap
apiVersion: v1
metadata:
  name: iron-ui-config
data:
  API_URL: Your-Iron_Address(eg:http://192.168.1.222:8080)
```
* Start iron-ui:
```
  kubectl create -f iron-ui-kubernetes
```
* Then you can access iron-ui by cluster ip(ip:4000) or node ip.
