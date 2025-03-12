# Install kubectl

## Pre-requisite: Install docker desktop

## Download the latest release of kubectl
```sh
curl -LO "https://dl.k8s.io/release/$(curl -s https://dl.k8s.io/release/stable.txt)/bin/windows/amd64/kubectl.exe"
```

## Add the binary to your PATH
```sh
move kubectl.exe C:\Windows\System32
```

## Verify the installation
```sh
kubectl version --client
kubectl version
```

## Install minikube

**download the latest release of minikube**
```sh
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-installer.exe)
```

**Run the installer and verify the status**
```sh
minikube version
minikube status
minikube start
minikube stop
```
