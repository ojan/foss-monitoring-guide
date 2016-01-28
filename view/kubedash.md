# Kubedash

https://github.com/kubernetes/kubedash

Performance analytics UI for Kubernetes Clusters.

The goal of Kubedash is to allow the user or an administrator of a Kubernetes cluster to easily verify and understand the performance of a cluster and jobs running within it through intuitive visualizations of aggregated metrics, derived stats and event patterns. 

It is not intended to be a general-purpose Kubernetes UI. Instead, kubedash uses multiple sources of information to summarize and provide high-level analytic information to users and to the cluster administrator.

## Some of the current features are:

- Resource utilization views of Cluster, Nodes, Namespaces, Pods and Containers for the past 1 hour.
- Derived stats for each resource over the past 1 day.
- Indications of containers with no resource limits.
- Future features include the following:

- Recommendations of resource limits for individual containers.
- Detecting and highlighting resource starvation in a cluster.
- Detecting and highlighting crash-looping and misbehaving containers.
- Support for other cluster management systems like CoreOS, Swarm, etc.