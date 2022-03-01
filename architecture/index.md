# Architecture


## Infrastructure Layer (Kubernetes)
Kynothon requires to be deployed on a Kubernetes cluster. The Kubenetes applications can be run on managed clusters (such as AWS EKS), self-hosted cluster (such as a [RaspberryPi cluster][1]) , or even locally using KinD or K3D.

The [Magic Lantern][2] repository contains tools to build a local kubernetes cluster with the necessary components to run the Kynothon system either using [KinD](https://kind.sigs.k8s.io/) or [K3D](https://k3d.io). 

## Applicative Layer (Magic-Lantern)
The system relies on OpenFaaS to provides the core of the functionnality such as distributed computation and auto-scaling.

## Orchestration Layer(Phantasmagoria)
Phantasmagoria is the collection of services that organizes the activation of the different functions from the functional layer using the applicative layer features.  

## Functional Layer (Zoethrope)
Zoethrope contains a collection of nano-services using the [OpenFaaS][3] templates.
 

[1]: <https://blog.alexellis.io/raspberry-pi-homelab-with-k3sup/> "Learn how to build your own Kubernetes Homelab with Raspberry Pi"

[2]: <https://github.com/Kynothon/Magic-Lantern> "Magic Lantern Repository"

[3]: <https://docs.openfaas.com/> "OpenFaaS - Serverless Functions Made Simple"

