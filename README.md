# kube-test

This repo has files that can be applied to a kube cluster and there will be some problems with them. The idea is to understand how a person identify and deals with them.

## Requisites
For this repo we will be using
* kind v0.24.0

But it should work with any type of kube cluster.

## Initial setup
Create a cluster
```
kind create cluster --wait 30s --config config.yaml
kubectl apply -f manifests
```

## Objective
Able to access `http://<some-host>/foo` and return the pod's name.

## Clean up
Delete cluster
```
kind delete cluster
```
