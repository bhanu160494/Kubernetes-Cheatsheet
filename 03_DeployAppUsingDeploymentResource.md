# Deploying Nginx Application using Kubernetes Deployment
This guide provides step-by-step instructions to deploy an Nginx application using a Kubernetes Deployment object. It covers creating the deployment, verifying the pod status, debugging, and understanding the advantages of using Deployment.

## Create deployment using YAML file
While deploying an application using the Deployment kind, Kubernetes creates Deployment >> ReplicaSet >> Pods (based on the number of replicas defined in the YAML file).

```sh
kubectl apply -f deploy.yaml
```

## Verify pod status
```sh
kubectl get all
kubectl get all -o wide
```

## Debugging cmds for deployment status
```sh
kubectl describe deploy nginx-deployment
kubectl logs nginx-deployment-85996f8dbd-5rfdv
```

## Verify running nginx application
We need to login into the cluster first because we didn't expose IP to the external world.
```sh
minikube ssh
curl <clusterIP>
```

**Note:** You can find the `clusterIP` by running `kubectl get svc`.

## Delete the pod
```sh
kubectl delete pod nginx
```

## Advantage of application deployment using Deployment kind.
- Auto-healing
- Auto-scaling
