# Deploy Charmed free5GC

## Requirements

free5GC must be installed on a Kubernetes cluster with the following specifications:

- **:material-kubernetes: Kubernetes**: A cluster with a total of a minimum of 6 vCPUs and 16 GB of RAM.
- **:material-ubuntu: Juju**: A Juju controller with access to the Kubernetes cluster

## Install free5GC

```bash
juju deploy free5gc-pcf --trust
```
