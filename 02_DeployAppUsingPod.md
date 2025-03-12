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
kubectl describe pod nginx
kubectl logs nginx
```

## Verify running nginx application
We need to login into the cluster first because we didn't expose ip to external world.
```sh
minikube ssh
curl <clusterIP>
```

## Delete the pod
```sh
kubectl delete pod nginx
```
## Disadvantages of application deployment with pod as k8s object.
- No auto-healing
- No auto-scaling
