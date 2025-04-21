## Pods
- K8s directly attract with pods only. 
- Pods are the smallest unit of K8s and inside pod containers are running in which the application deployed.

## Create pod using yaml file.
```sh
kubectl apply -f resources/pod.yaml
```

## Verify pod status
```sh
kubectl get pods
kubectl get pods -o wide
```

## Debugging cmds for pod status
```sh
kubectl describe pod nginx // nginx is the name of pod
kubectl logs nginx
```

## Verify running nginx application
We need to login into the cluster first because we didn't expose ip to external world.
```sh
minikube ssh #since we are using minikube as cluster 
curl <Internal IP of pod>

kubectl exec -it nginx -- /bin/bash #For login into pod
kubectl exec -it nginx -c <container_name> -- /bin/bash #For login into the particular container if multiple containers are running inside pod 
curl <Internal IP of pod>
```

## Delete the pod
```sh
kubectl delete pod nginx
```
## Disadvantages of application deployment with pod as k8s object.
- No auto-healing
- No auto-scaling
