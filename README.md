# Kubernetes Ecosystem

This repository puts together all the resources related to Kubernetes together.

## Table of Contents

* [What is?](#what-is)
* [Concepts](#concepts)
   * [Pods](#pods)
   * [Nodes](#nodes)
   * [Services](#services)
   * [Deployments](#deployments)
* [Configurations](#configurations)
* [Secrets](#secrets)
* [Common Kube Commands](#common-kube-commands)
* [Supporting Tools](#supporting-tools)
    * [Minikube](#minikube)
    * [Kubectx](#kubectx)
    * [Kubetail](#kubetail)
    * [Stern](#stern)
    * [Fblog](#fblog)

### <a name="what-is"></a>What is?

Kubernetes is a container orchestration framework. Scheduling and general Management of containers (commonly Docker containers).

### <a name="concepts"></a>Concepts

+ Pods
+ Nodes
+ Services
+ Deployments
+ ConfigMaps
+ Sealed Secrets
+ Volumes / Persistent Volumes (PV) & Claims (PVC) 

#### <a name="pods"></a>Pods

Pods are logical groupings of Containers in Kubernetes. They provide an abstraction over Containers. Pods can contain one or many containers.

#### <a name="Nodes"></a>Nodes

Nodes are locations where the pods reside. These can be Physical servers or Virtual Machines (VMs).

#### <a name="Services"></a>Services

Services are another higher level of abstraction over Pods which provides a logical grouping of pods. It gives features such as Load Balancing.

#### <a name="deployments"></a>Deployments

Deployments are a management way of managing a "Deployment" in Kubernetes. Specifying a deployment allows Kubernetes to manage the lifecycle of the pods and services for your container. To be able to automatically scale up or down depending on specified requirements (i.e. to ensure the number of pods matches the number of 'replicas' as defined in the deployment descriptor yaml file.) For e.g. if you delete your pods, Kubernetes will ensure the system always adheres to the scaling rules definied in that deployment descriptor yaml file.

### <a name="configurations"></a>Configurations

Configuration is implemented using ConfigMaps. These are key/value pairs of configuration properties stored inside a map data structure within Kubernetes.

### <a name="secrets"></a>Secrets

Secrets represents sensitive data (key bits of information) such as passwords, important keys, usernames etc.
In Kubernetes you make use of "Sealed Secrets" to securely store sensitive data inside Kubernetes.

### <a name="common-kube-commands"></a>Common Kube Commands

See [https://github.com/colinbut/kubernetes-commands-cheatsheet](https://github.com/colinbut/kubernetes-commands-cheatsheet)

### <a name="supporting-tools"></a>Supporting Tools
- Kubectl (Kubernetes CLI)
- minikube
- Kubectx
- Kubetail
- Stern
- Fblog

#### <a name="minikube"></a>Minikube

[Minikube](https://github.com/kubernetes/minikube) allows you to run a Kubernetes cluster locally. Minikube only supports a single node cluster. It is a brilliant way to get started with Kubernetes to learn the ropes. Read [here](https://kubernetes.io/docs/setup/minikube/) for more details.

#### <a name="kubetail"></a>Kubectx

[Kubectx](https://github.com/ahmetb/kubectx) is a tool that allows you to quickly switch between different Kube clusters and namespaces.

#### <a name="kubetail"></a>Kubetail

[Kubetail](https://github.com/johanhaleby/kubetail) is a simple tool implemented as a bash script that will allow you to tail logs from multiple Kubernetes pods in real-time instantly.

#### <a name="stern"></a>Stern

[Stern](https://github.com/wercker/stern) is another multi-pod & container log tailing tool. It is quite good and quite advanced than Kubetail. But my verdict is Kubetail might be a bit similar to use and ideal for the most simple use case.

#### <a name="fblog"></a>Fblog

[fblog](https://github.com/brocode/fblog) is simple command line JSON log viewer which is ideal to be used with the other log tailing tools above. It is a tool written in Rust.
