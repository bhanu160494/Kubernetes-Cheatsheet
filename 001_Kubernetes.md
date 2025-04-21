# Need of Kubernetes:
- Containers created by docker are not communicate with each other so K8s comes to wrap the container inside pod and assign external ip to those pods for communincation.
- Autoscaling and load balancing is not possible in docker container.

# What is Kubernetes
- K8s is an orchestration tool (container management tool).
- It's an open source tool which automates the container deployment in isolated env, perform container scaling and load balancing.
- K8s has inbuild tool for managing and logging the errors.

# Features:
- Platform independent (manage all the containers created by differnt tools like Docker, Rocket, ContainerD)
- Autoscaling
  * Horizontal (Increase the resouces allocation to the cluster. Limited upto the resource available in the node)
  * Vertical (Add more nodes and cloning the existing deployment to them)
- Load Balancing
- Roll back
- Health monitoring of containers
