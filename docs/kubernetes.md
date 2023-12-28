# Kubernetes

## Clusters

### Quick reference

* see what clusters have been set up, including which one is current
  ````shell
  kubectl config get-contexts
  ````
* switch current cluster
  ````shell
  kubectl config use-context the-other-cluster
  ````
* try accessing a cluster without switching the current one
  ````shell
  kubectl --cluster the-other-cluster --user the-user-name-in-config cluster-info
  ````
* see all config
  ````shell
  less ~/.kube/config
  ````

### Setting up cluster access

* [in K3s](https://docs.k3s.io/cluster-access)
* Note that the user name in the config file isn't meaningful - it's just used to wire the various config together. So you should change it so that it's specific to the cluster.
