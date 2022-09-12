# deploy-thanos-kubernetes

Example thanos deployment on kubernetes.  Code for this repo is taken from [kube-thanos](https://github.com/thanos-io/kube-thanos) and slight modifcations made.

## Configure thanos on kubernetes cluster

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
