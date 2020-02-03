# BASIC CONECPTS

Kubernetes work for managing and ochestrating containers. For it, kubernetes uses 2 key functions that are 'container image format' and 'cgroups'.

## Container

## Pod

Pod is smallest unit that managed by kubernetes and it makes system as a base unit. Pod is consist of one or more containers and associated informations. Pod is easily created and deleted, so it has very small life-time. Pod guarantee next 4 factors.

* Containers in pod runs in the same node.
* Containers in same pod use same network and can communicate each others through network.
* Containers in same pod can share storage that are connected with pod.
* Pod has lifecycle, if it re-created then it runs in the first created node.

### pod lifecycle

https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle/

### probes

Kubernetes has two kinds of probes. livenessProbe checks container running or not. readenessProbe checks container can service or not.

https://kubernetes.io/docs/tasks/configure-pod-container/configure-liveness-readiness-startup-probes/

## Namespace

namespace limit to resources use like CPU, memory. and affect to DNS and access control policy.

## controller

## network

## ReplicaSet

RelicaSet is higher concepts of pod. It define number of running pods in same time. ReplicaSet inspect status of pod and do effort to maintain number of running pods.

## Deployment

Deployment is higher concepts of ReplicaSet.
