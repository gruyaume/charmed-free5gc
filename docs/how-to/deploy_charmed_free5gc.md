# Deploy Charmed free5GC

## Requirements

free5GC must be installed on a Kubernetes cluster with the following specifications:

- **:material-kubernetes: Kubernetes**: A cluster with a total of a minimum of 6 vCPUs and 16 GB of RAM.
- **:material-ubuntu: Juju**: A Juju controller with access to the Kubernetes cluster

## Getting Started

Install microk8s with the necessary add-ons:

```bash
snap install microk8s --classic
microk8s enable dns
microk8s enable storage
microk8s enable community
microk8s enable multus
```

## Install free5GC

```bash
juju deploy free5gc-amf-operator --trust --channel=edge
juju deploy free5gc-pcf-operator --trust --channel=edge
```
