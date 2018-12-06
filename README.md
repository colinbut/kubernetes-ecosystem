# Kubernetes Ecosystem

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

See [TBD]

## Supporting Tools
- Kubectl (Kubernetes CLI)
- Kubectx
- Kubetail
- minikube
- Stern
- Fblog
