# deploy-thanos-kubernetes

Example thanos deployment on kubernetes to use along with [kube-prometheus](https://github.com/prometheus-operator/kube-prometheus#quickstart). Code for this repo is taken from [kube-thanos](https://github.com/thanos-io/kube-thanos) and slight modifcations made.

## Configure thanos on kubernetes cluster

Create namespace named 'monitoring' if doesn't exist (This example project is created to use along with [kube-prometheus](https://github.com/prometheus-operator/kube-prometheus#quickstart), so "monitoring" namespace should be already created after following instructions over there)

```bash
kubectl create ns monitoring
```

```bash
kubectl apply -f manifests
```

## Compile yourself

### Pre-requistes

- [jsonnet](https://github.com/google/jsonnet)
- [jsonnet-bundler](https://github.com/jsonnet-bundler/jsonnet-bundler#install)
- [gojsontoyaml](http://github.com/brancz/gojsontoyaml)

### Generate manifest files

```bash
./build.sh
```
