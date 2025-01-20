### Create ConfigMaps like this:

### Declarative

```shell
kubectl create -f file.yml
```

file.yml =

```shell
APP_COLOR: blue
APP_MODE: prod
```

### Imperative

```shell
kubectl create configmap app-config --from-literal=APP_COLOR=blue --from-literal=APP_MODE=prod
```

```shell
kubectl create configmap app-config --from-file=app_config.properties
```
