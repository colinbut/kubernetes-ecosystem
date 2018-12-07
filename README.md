# Kubernetes Ecosystem

This repository puts together all the resources related to Kubernetes together.

## What is?

Kubernetes is a container orchestration framework. Scheduling and general Management of containers (commonly Docker containers).

## Concepts

+ Pods
+ Nodes
+ Services
+ Deployment
+ ConfigMaps
+ Sealed Secrets
+ Volumes / Persistent Volumes (PV) & Claims (PVC) 

## Configuration

Configuration is implemented using ConfigMaps. These are key/value pairs of configuration properties stored inside a map data structure within Kubernetes.

## Secrets 

Secrets represents sensitive data (key bits of information) such as passwords, important keys, usernames etc.
In Kubernetes you make use of "Sealed Secrets" to securely store sensitive data inside Kubernetes.

## Common Kube commands

See [https://github.com/colinbut/kubernetes-commands-cheatsheet](https://github.com/colinbut/kubernetes-commands-cheatsheet)

## Supporting Tools
- Kubectl (Kubernetes CLI)
- minikube
- Kubectx
- Kubetail
- Stern
- Fblog

### Minikube

[Minikube](https://github.com/kubernetes/minikube) allows you to run a Kubernetes cluster locally. Minikube only supports a single node cluster. It is a brilliant way to get started with Kubernetes to learn the ropes. Read [here](https://kubernetes.io/docs/setup/minikube/) for more details.

### Kubectx

[Kubectx](https://github.com/ahmetb/kubectx) is a tool that allows you to quickly switch between different Kube clusters and namespaces.

### Kubetail

[Kubetail](https://github.com/johanhaleby/kubetail) is a simple tool implemented as a bash script that will allow you to tail logs from multiple Kubernetes pods in real-time instantly.

### Stern

[Stern](https://github.com/wercker/stern) is another multi-pod & container log tailing tool. It is quite good and quite advanced than Kubetail. But my verdict is Kubetail might be a bit similar to use and ideal for the most simple use case.

### Fblog

(fblog)[https://github.com/brocode/fblog] is simple command line JSON log viewer which is ideal to be used with the other log tailing tools above. It is a tool written in Rust.
