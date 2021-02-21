# The kube

Project explains how Kubernetes manages the containerized applications.

Understanding_Kubernetes folder consist all the resources about presentation and commands used during the session.

My-Web-Api folder has the API project that is used to create a docker image.

## Kubernetes and it's components

Kubernetes basically has two main component
Control Panel
and 
List of Nodes

### Control Panel

Control panel has following sub components

#### API Server

Exposed the REST based API to an end users ( Could be kubectl or Nodes requesting or accessing resources ) to get the status of kubernetes objects and resources and it's state.

#### Scheduler

Helps assigning the newly created pod to the node based upon pod's resource limit specifications

### List of Nodes

List of nodes are the one that holds applications running under containers

#### KubeLet

Every node has one kubelet that makes sure that each node is health and also reserve the pod specification resource limit for the pod to be used only for that pod.
