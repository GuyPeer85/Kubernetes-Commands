Special commands:
---------------

**patch**
- `kubectl patch <pod name> -p '{"spec":{"containers":[{"name":"nginx","image":"nginx:1.11"}]}}`

is a command used to modify an existing Kubernetes pod by patching its specification with the provided JSON or YAML data. The example updates the image of the nginx container to version 1.11

**taint nodes**
- `kubectl taint nodes <name node> key=value:NoSchedule`
  
his command is used to add a taint to a node in a Kubernetes cluster, which will prevent certain pods from being scheduled on that node.

**label pod**
- `kubectl label pod <pod name> app=backend`

This command is used to add, modify or remove labels from Kubernetes resources, such as pods or deployments.

**drain**
- `kubectl drain <node name> --ignore-daemonsets`

This command is used to gracefully remove a node from a Kubernetes cluster, moving the workloads to other nodes before shutting down the node.

**port-forward**
- `kubectl port-forward <pod name> <target port>:<port>`

This command is used to forward a local network port to a specific port on a pod in Kubernetes, allowing you to access services running within the pod from your local machine.

**expose deployment**
- `kubectl expose deployment <deployment name> --type=<LoadBalancer / NodePort> --port=<number> --target-port=<number>`

This command is used to create a new Kubernetes service for a specific deployment or pod, which exposes it to the network.

**annotate pod**
- `kubectl annotate pod <pod name> description="This pod contains my backend API"`

This command is used to add or update the annotations of a specific Kubernetes resource.
