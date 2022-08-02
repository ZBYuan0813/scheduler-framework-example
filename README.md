# sample-scheduler-framework

This repo is a sample for Kubernetes scheduler framework.

## Deploy

```shell
$ kubectl apply -f deploy/sample-scheduler.yaml
```

## Test
```shell
$ kubectl apply -f deploy/test-scheduler.yaml
```

Then watch sample-scheduler pod logs.

## Test local IDE
go run main.go --kubeconfig ~/.kube/config --leader-elect-resource-name sample-scheduler --v 3 --scheduler-name sample-scheduler