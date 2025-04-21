# Architecture:

- Kubernetes follows client-server architecture.
- We have master nodes and worker nodes which contains different components for execution separate tasks.
- Checkout `/resources/Architecture of K8s.jpg` file for details

# Various components:
- Master node
  * kube-api-server (provide CLI to interact with k8s resources)
  * kube scheduler (assign nodes to new created pods)
  * ETCD (behave like a db which have all cluster related data in key-value form)
  * Controller manager (responsible for managing state of clusters)
- Working node
  * kubelet (behave as agent which make sure tha containers are running inside pod)
  * kube proxy (assign IP to the pod and maintain n/w rules for communication with pod)
  * container runtime (tools which are responsible for running containers eg Docker)
  
