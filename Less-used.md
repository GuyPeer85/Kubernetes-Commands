Less used commend
=================

**Namespace** - 
- `kubens <name>`
- `kubens <create / delete / describe > namespace <name>`
- `kubens get <pod / deployments / services > --namespace=<name>`
- `kubens config view --minify --output 'jsonpath={..namespace}`

A utility to switch between Kubernetes namespaces. It allows you to list the available namespaces and switch to a different one.

**Set** - used to modify existing resources by changing the values of one or more of their fields. It can be used to update or patch resources such as pods, deployments, services, and replicasets by changing their configurations, annotations, or labels.
***all list in kubectl set –help****
- `kubectl set image replicaset my-replicaset nginx=nginx:1.13`
- `kubectl set  < env / resources / dry-run / serviceaccount / volume / selector / subject / status >`
- `kubectl.kubernetes.io/last-applied-configuration`

is a command used to update the image of the container named nginx running in a Kubernetes ReplicaSet named my-replicaset. The specified image nginx:1.13 is pulled from a container registry and replaces the existing image. This command can be used to perform rolling updates of container images in a ReplicaSet.

**Scale** - scaling refers to the process of increasing or decreasing the number of replicas (or instances) of a specific resource, such as pods, deployments, replica sets, or stateful sets.
- `kubectl scale replicaset < replicaset-mane> --replicas <replica-count>`
- `kubectl scale deployment <deployment-name> --replicas=<replica-count> --current-replicas=<current-replicas>`
- `kubectl scale statefulset <statefulset-name> --replicas=<replica-count> --current-replicas=<current-replicas>`

is a command used to scale the number of replicas in a Kubernetes ReplicaSet named <replicaset-name>
  
**f**
